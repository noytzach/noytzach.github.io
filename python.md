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

## executable
```
def inc(x):
   return x+1
   
if __name__ == "__main__":
   print(inc(argv[0]))
```
