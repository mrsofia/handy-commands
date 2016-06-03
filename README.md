# Handy terminal commands for OS X/Linux

### Searching for a dir or file
```markdown
find / -type d -iname 'file-or-dir-name'
```

- `type` is not mandatory, `d` indicates we're searching for a dir
- `-iname` ignores case, `-name` doesn't
- `/` indicates dir to search in, in this case we're searching from root
- `file-or-dir-name` can mix regexes like `*.php`

### Zipping a dir or file
```
zip zippedfilename.zip file1 file2
zip file.zip dir1
zip -r file.zip /path/to/your/dir/
zip -r file.zip "*.java"
```

### grepping for a string and returning the number of lines it is used (useful for checking logs)
```
grep -ir '<your-string>' --exclude=*svn* | awk '{ print } END { print NR }'
```
