# Xcelium cheaetsheet

## list all instances into instances.txt
```
exec echo [foreach i [find  * -instances -recursive all] {puts [describe $i -verbose]}] > instances.txt
```
