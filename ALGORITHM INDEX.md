# Sample index.uati
```
#add:a,b,OUT
@example lang a: num a, num b, num OUT
a>
b>
+
OUT<
@end

@example lang b: var a, var b, ret OUT
add(a, b) {
    return a+b
}
@end

#end


$example lang a

%transpiler:example lang b
%global
%usection:init vars:
char STACK[]
%sectionend
%globalend

$end
```