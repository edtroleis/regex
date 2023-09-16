# Get valid ipv4

## Regex

```regex
/^((25[0-5]|(2[0-4]|1\d|[1-9]|)\d)\.?\b){4}$/gm
```

## Test

```
# incorrect
192.268.0.1
1.333.1.1
192.168.0.256
256.256.256.256

# correct
192.168.0.1
127.0.0.1
10.0.0.255
10.11.12.0
255.255.255.255
0.0.0.0
```

# Notes

- https://regex101.com/
- https://developer.hashicorp.com/terraform/language/modules/sources#github
