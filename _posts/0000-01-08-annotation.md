---

title: "" 
---

- **How...**
  - how does javac know the anontation processors?
    - *built-in annotations e.g. [@Override in java/lang](https://github.com/openjdk/jdk/blob/master/src/java.base/share/classes/java/lang/Override.java)*
    - For a jar file, you should have `META-INF/services/javax.annotation.processing.Processor` with processor name [sample](https://riptutorial.com/java/example/19926/compile-time-processing-using-annotation-processor)
    - *customized annotations [sample in source code](https://github.com/openjdk/jdk/blob/master/test/langtools/tools/javac/processing/ReportOnImportedModuleAnnotation/mods-src1/annotation/annotation/ModuleWarn.java)*
  - how do customized anontation processors know anontations?
    - *scan elements*
    - *processors annotated with `@SupportedAnnotationTypes("path.SupportedAnnotationType")` [sample in source code](https://github.com/openjdk/jdk/blob/master/test/langtools/tools/javac/processing/ReportOnImportedModuleAnnotation/mods-src1/processor/processor/ModuleWarnProcessor.java)*
