<h2 align="center">Hi! I'm Lucas. <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px"></h2>

<!--   <img align="right" alt="GIF" src="https://github.com/lucaslima777/lucaslima777/blob/main/code.gif?raw=true" width="500" height="320" /> -->
  
```kotlin
lucas.apply {
        occupation = "Mobile Software Engineer".plus(Pleno)
        skills = listOf(Kotlin, Java, Gradle, Swift, Git)
        currentlyLearning = mutableListOf("Flutter", "BackEnd", "Neuroscience")
        toolsUsing = mutableListOf("Jenkins", "AWS", "Splunk", "SonarQube", "Jira")
        likeCoffe = true
    }.runCatching {
        drinkCoffee()
        toWork()
        drinkCoffee()
        fixBug()
        drinkCoffee()
    }.onSuccess {
        deploy()
    }.onFailure { error ->
        when(error) {
            is OutOfMemoryError -> searchOnStackOverflow(error)
            is ExitException -> waitMeToComeBack()
            is StackOverflowError -> {
                // FIXME
            }
        }
        Logger.logMsg(ERROR, error.message)
    }.also {
        toStudy()
        toSleep()
    }.repeat(Monday..Friday)
```
