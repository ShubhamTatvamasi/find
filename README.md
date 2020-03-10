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

find files modified in last 10 minutes
```bash
find . -type f -mmin -10
```

find files that was modified more than 10 minutes ago
```bash
find . -type f -mmin +10
```

find files that was modified more than 1 minutes ago and less than 5 minutes ago
```bash
find . -type f -mmin +1 -mmin -5
```

find files modified less than 10 days ago
```bash
find . -type f -mtime -10
```

find files modified more than 10 days ago
```bash
find . -type f -mtime +10
```
> `-amin` and `-cmin` can also be used
---


find files more than 5 megabyte
```bash
find . -type f -size +5M
```
> use `k` for kilobytes and 'G' for gigabytes

find empty files
```bash
find . -type f -empty
```
> you can also search for empty directories by giving `-type d` flag

find files and directories with 777 permission
```bash
find . -perm 777
```

find the file and execute the command
```bash
find . -type f -name "apple" -exec cat {} +
```

find files only in current directory 
```bash
find . -type f -maxdepth 1
```
