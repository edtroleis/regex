# Terraform regex

## Get repository and tag from Terraform modules

### Regex

```regex
/^\s*source\s*=\s*\"git::(.*.git\?ref=(.*))\"$/gm
```

### Test

```terraform
module "vpc" {
  source = "git::https://example.com/vpc.git"
}

module "storage" {
  source = "git::ssh://username@example.com/storage.git"
}

module "storage2" {
  # source = "git::ssh://username@example.com/storage.git"
  source = "git::ssh://username@example.com/storage.git"
}


# select a specific tag
module "vpc" {
  source = "git::https://example.com/vpc.git?ref=v1.2.0"
  # source = "git::https://example.com/vpc.git?ref=v1.2.0"
}

# directly select a commit using its SHA-1 hash
module "storage" {
  source = "git::https://example.com/storage.git?ref=51d462976d84fdea54b47d80dcabbf680badcdb8"
}
```

# Notes

- https://regex101.com/
- https://developer.hashicorp.com/terraform/language/modules/sources#github
