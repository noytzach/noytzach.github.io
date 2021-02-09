# Verilog-Mode Cheatsheet

### Finding Modules
```
// Local Variables:
// verilog-library-directories:("." "subdir" "subdir2")
// verilog-library-files:("/some/path/technology.v" "/some/path/tech2.v")
// verilog-library-extensions:(".v" ".h")
// End:
```

### Changing case
```
    .apb\(.*\) (@"(upcase \\"\1\\")"[]), //or downcase
```

### Ignore
```
// Local Variables:
// verilog-auto-input-ignore-regexp: "VSS"
// verilog-auto-output-ignore-regexp: "unconnected.*"
// END:

```

### Propagate Parameters
```
// Local Variables:
// verilog-auto-inst-param-value:t
// END:
```

