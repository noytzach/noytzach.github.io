# Bash Cheatsheet
## Redirection
```
cmd > out.txt 2> err.txt # redirect stdout to out.txt and stderr to err.txt
cmd > out.txt 2>&1       # redirect both to out.txt
```

## Loop files
```
for f in *.txt
do
   echo $f
done
```
