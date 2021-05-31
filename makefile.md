# Makefile Cheatsheet

based on [this](https://devhints.io/makefile)

## magic variables
```
main.o: main.c main.h
  $@   # "main.o" (target)
  $<   # "main.c" (first prerequisite)
  $^   # "main.c mian.h" (all prerequisites)
```  

```
%.o: %.c
  $*   # the 'stem' with which an implicit rule matches ("foo" in "foo.c")
```

## find files
```
verilog_files  := $(wildcard rtl/*.v)
all_files := $(shell find rtl -name "*")
```

## assignments
```
uglify = $(uglify)        # lazy assignment
compressor := $(uglify)   # immediate assignment
prefix ?= /usr/local      # safe assignment
hello += world            # append
```

## substitution
```
file     = $(SOURCE:.cpp=.o)   # foo.cpp => foo.o
```

## command prefix
```
-cmd       # ignore error
@cmd       # do not print command
```

## grouped targets
see [here](https://www.gnu.org/software/make/manual/html_node/Multiple-Targets.html)
```
foo bar biz &: baz boz
   echo hello
```
