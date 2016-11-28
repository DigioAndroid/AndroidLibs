# Testing tips

## General
* Method names in test. Must have the following format: "should" + "[action]" + "when" + "[condition]"<br>
  
  <b>action</b> = Action or actions to be taken when the condition is executed.<br>
  <b>condition</b> = Environment to take action <br>
  
  <b>Example:</b><br>
  `public void shouldGetLocalDataWhenCreatePresenter(){
  }`
  
* Tests must conform to the next structure: Given -> When -> Then

## Kotlin
### Some useful articles about Testing with Kotlin
* [Using Kotlin For Tests in Android](https://medium.com/@sergii/using-kotlin-for-tests-in-android-6d4a0c818776)

### Tips
* In a Kotlin test, instead of using *when* method from Mockito library, which is a reserved keyword from Kotlin, better use ***whenever*** (for that, you should add to your build gradle mockito-kotlin library dependency).
* If we want to mock an answer from a method, and we want a new instance each time. Use ***thenAnswer{object}*** instead *when...thenReturn(object).
* En lugar the usar los asserts tradicionales de junit, es MUY recomendable usar los asserts de la librería Thruth the Google, que los hace mas legibles así como un reporte de los test que han fallado mas claro.

## Spock
