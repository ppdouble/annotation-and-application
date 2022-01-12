---

title: "" 
center: false

---

- Reflection: 
  - *introspection* 
  - *the ability of a program to examine its own structure at runtime*

----------------
- **Static**
  - *compile-type checking*

`Foo myObject = new Foo();`
-------------

- **Dynamic**
  - *runtime checking*

```Java
Object myObject = Class.forName("Foo").getConstructor().newInstance();
```
