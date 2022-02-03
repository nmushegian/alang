
A is structs and pointers. C is structs and pointers and undefined behavior.

- C-like core: machine num types, pointers, structs, unions, function pointers, labels-as-values
  - partial effect types: functions are colored with 'tags' that cannot be discharged
- - strictly for static analysis
- length-prefixed arrays, but has unsafe access syntax
- modern sensibilities
- - multiple return
- - type signatures make sense
- - modules and lockfiles



```
+e  possibly has effect
-e  necessarily not has effect
:   type
  #   struct
  |   union
  $   array
\/  proc
{}  block
&   ref
*   deref
```

effects:

```
mem
memread
memwrite
syscall k1, k2, ...
asm
goto
floats
ptrsize k
```
