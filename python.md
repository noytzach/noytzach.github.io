# Python Cheatsheet

## shebang
```
#!/usr/bin/env python3
```

## read lines of file
```
with open('file.txt') as fp:
   lines = fp.read().splitlines() # get rid of \n
```

## iterate over dictionary
```
for k, v in d.items():
   print(k, '->', v)
```

## executable
```
def inc(x):
   return x+1
   
if __name__ == "__main__":
   print(inc(argv[0]))
```

## print no newline
```
print('text here', end='', flush=True) #flush to be printed immediately
```

## enumerate
```
for count, value in enumerate(values):
   print(count, value)
```

## add to import path
```
import sys
sys.path.insert(0, "/path/to/package")
import package
```
