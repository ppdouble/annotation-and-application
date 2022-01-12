---

title: "" 
center: false

---

- Reflection: 
  - *introspection* 
  - *the ability of a program to examine its own structure at runtime*

- **Static**

```Java
Foo myObject = new Foo();
```

  - compile-type checking


- **Dynamic**

```Java
Object myObject = Class.forName("Foo").getConstructor().newInstance();
```
  - runtime checking
