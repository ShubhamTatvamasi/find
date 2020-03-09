# find

search all json files recursively
```bash
find . -name "*.json"
```

find and delete
```bash
find . -name ".DS_Store" -exec rm -rf {} \;
```

search only for directories
```bash
find . -type d
```

search only for files
```bash
find . -type f
```

search for files - case insensitive
```bash
find . -type f -iname "test*"
```
