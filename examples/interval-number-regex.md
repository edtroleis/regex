# Get number from 0 to 255

## Regex

```regex
/\b(\d{1,2}|1\d{2}|2[0-4]\d|25[0-5])\b/gm
```

## Test

```
0 1 2 5 10 150 199 200 201 202 2030 240 250 254 255 256 257 300 400 500 1000
```

# Notes

- https://regex101.com/
- https://developer.hashicorp.com/terraform/language/modules/sources#github
