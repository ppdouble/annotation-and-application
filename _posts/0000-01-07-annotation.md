---

title: "" 
---

- **How...**
  - Annotations definition
    - *built-in annotations e.g. [@Override in java/lang](https://github.com/openjdk/jdk/blob/master/src/java.base/share/classes/java/lang/Override.java)*
    - *customized annotations [sample in source code](https://github.com/openjdk/jdk/blob/master/test/langtools/tools/javac/processing/ReportOnImportedModuleAnnotation/mods-src1/annotation/annotation/ModuleWarn.java)*
  - Annotation processors
    - *built-in processor [com/sun/tools/javac/processing/JavacProcessingEnvironment.java](https://github.com/openjdk/jdk/blob/master/src/jdk.compiler/share/classes/com/sun/tools/javac/processing/JavacProcessingEnvironment.java#L251), [checkOverride](https://github.com/openjdk/jdk/blob/master/src/jdk.compiler/share/classes/com/sun/tools/javac/comp/Attr.java#L1016), [overrideType](https://github.com/openjdk/jdk/blob/master/src/jdk.compiler/share/classes/com/sun/tools/javac/code/Symtab.java#L573)* 
    - *customized annotation processor, sample in [source code](https://github.com/openjdk/jdk/blob/master/test/langtools/tools/javac/processing/ReportOnImportedModuleAnnotation/mods-src1/processor/processor/ModuleWarnProcessor.java) and [lambok](https://github.com/projectlombok/lombok/blob/master/src/core/lombok/javac/apt/LombokProcessor.java#L328)*

