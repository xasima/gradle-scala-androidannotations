# gradle-scala-androidannotations

A sample gradle android project with androidannotations, multidex and scala plugin. It's works ok from Android Studio 1.0.1

This project was originally created to address     [androidannotations#521](https://github.com/excilys/androidannotations/issues/521) warnings, that had been fixes by [gradle-android-scala-plugin v.1.3.2](https://github.com/saturday06/gradle-android-scala-plugin/issues/47).
 
 # Configure

You may need to create local.properties file in the project root with the pointer to sdk installation

`sdk.dir=/opt/android-sdk-linux`

# Use 

Try `./gradlew clean assembple` or `./gradlew :app:compileProdPublicBetaJava` to see that this compiles well. 

 