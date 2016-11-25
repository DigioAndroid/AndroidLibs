# Testing tips

## Kotlin
* In a Kotlin test, instead of using *when* method from Mockito library, which is a reserved keyword from Kotlin, better use ***whenever*** (for that, you should add to your build gradle mockito-kotlin library dependency).
* If we want to mock an answer from a method, and we want a new instance each time. Use ***thenAnswer{object}*** instead *when...thenReturn(object).

