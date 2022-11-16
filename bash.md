# Bash Cheatsheet
## Redirection
```
cmd > out.txt 2> err.txt # redirect stdout to out.txt and stderr to err.txt
cmd > out.txt 2>&1       # redirect both to out.txt
```

## Loop files
```
shopt -s nullglob      # in case no *.txt files 
for f in *.txt
do
   echo $f
done
```

## Infinite loop
```
while true; do echo 'Hit CTRL+C'; sleep 1; done
```
