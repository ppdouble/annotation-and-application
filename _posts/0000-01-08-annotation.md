---

title: "" 
---

- **How...**
  - how do customized anontation processors know anontations?
    - *javac scan elements*
    - *processors annotated with @SupportedAnnotationTypes("path.SupportedAnnotationType") [sample in source code](https://github.com/openjdk/jdk/blob/master/test/langtools/tools/javac/processing/ReportOnImportedModuleAnnotation/mods-src1/processor/processor/ModuleWarnProcessor.java)*
    - *Using `getElementsAnnotatedWith(customized-annotation.class)` in method process()*
