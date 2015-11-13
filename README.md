# Handy terminal commands for OS X/Linux

### Searching for a dir or file
```markdown
find / -type d -iname 'file-or-dir-name' 
```

- `type` is not mandatory, `d` indicates we're searching for a dir
- `-iname` ignores case, `-name` doesn't
- `/` indicates dir to search in, in this case we're searching from root
- `file-or-dir-name` can mix regexes like `*.php` 
