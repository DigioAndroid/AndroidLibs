# Testing tips

* In a test in Kotlin instead of using *when* word, which is reserved, better use ***whenever***.
* If we want to mock an answer from a method, and we want a new instance each time. Use ***thenAnswer{object}*** instead *when...thenReturn(object).
