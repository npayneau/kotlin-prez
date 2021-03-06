---
Kotlin presentation

![Logo](https://kotlinlang.org/assets/images/twitter-card/kotlin_800x320.png)
---
## Who am I ?

- Nicolas Payneau |
- 8 years experience |
- Code lover |
- Follow me on twitter @npayneau |
---
## What is this Kotlin ?

* Statically typed programming language for JVM and Android 
* Running in JVM
* Supports both OO and functional styles
---
## What is this Kotlin ?

* Started as internal language “Project Kotlin” at Jetbrains in July 2010
* Kotlin 1.0 since Feb 2016
* Open-Source, Apache License
* Named after an island in the Gulf of Finland 
---
## What is this Kotlin ?

* Since 1.0 release: multiple maintenance releases up to 1.0.7
* 1.1 was released in Feb 2017, now at 1.1.1
* Kotlin/JS is a ﬁrst-class deployment/compilation target now
* Strong community, lots of interesting frameworks, awesome support from Jetbrains 
---
## The advantages of kotlin

| ------------ | --------------- | ------------ |
| Immutability |String templates  | Null safety |
| Properties and Fields | Data classes | Extension functions | 
|Syntactic sugar | Type inference | Lambdas |
|Collection API | Type-safe builders

---
## IMMUTABILITY

* Support for mutable and immutable variables, properties and ﬁelds 
* Keywords var and val 
  * val - immutable (recommended)
  * var - mutable 
* Similar concept applies for class properties 

```java
val a: Int = 1
val b = 1 
val c: Int c = 1 
val x = 23 // fails x += 1 
```

---
## STRING TEMPLATES 

* Kotlin Strings can contain template expressions
* String templates start with a $ character and 
 * can contain simple references such as ```$s```, as well as 
 * complex expressions in curly braces: ```${s.length}```

```java 
 val s = "abc" 
 val str = "$s.length is ${s.length}"
 
 Output: abc.length is 3 IDIOMS & LANGUAGE PATTERNS 
```
---
## NULL SAFETY
* An explicit way to deal with NPEs
* Nullable types vs non-nullable types:
 * String: no nullable
 * String?: nullable 
* Handle manually
* Use Safe Call operator ?. 
* !! operator to allow/trigger a NPE 

```java
// Won't compile 
var lastName: String = null 

// Will compile 
var lastNameNullable: String? = null

// Will also not compile 
println(lastNameNullable.length) 

// Option 1 (-1) 
println(if (lastNameNullable != null) lastNameNullable.length else -1) 

// Option 2 (null) 
println(lastNameNullable?.length) 

// Option 3 (NPE) 
println(lastNameNullable!!.length) 
```

## Thanks 

---

## References

* [Kai Koenig](https://fr.slideshare.net/AgentK/2017-kotlin-now-more-than-ever) , Software Architect at Ventego Creative Ltd

