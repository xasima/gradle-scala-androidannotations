# gradle-scala-androidannotations
A sample gradle android project with androidannotations, multidex and scala plugin

This project is created to address some    [androidannotations#521](https://github.com/excilys/androidannotations/issues/521) warnings.
We didn't try to write down scala code directly in main/scala.
We may use appropriate scala libraries via java code in this project.
If you need to test some scala code in android project as well, please use
a pure IntelliJ-CE with scala facet installed.

# Install

To test the warning, you may need to create local.properties file in the project root with the pointer to sdk installation

```sdk.dir=/opt/android-sdk-linux```


# Issue

Please perform

* `./gradlew :app:compileProdPublicBetaJava` to observe the warning below directly, or
* `./gradlew clean assemble` to scroll to appropriate favor (beta) and build type (release) output

You need to see the following warning

```
Note: Initialize AndroidAnnotations 3.3-SNAPSHOT with options {androidManifestFile=/home/weblab/dev2/enrollment-mobile-android/app/build/intermediates/manifests/full/prod/publicBeta/AndroidManifest.xml, resourcePackageName=pan.enrollforecast.activity}

warning: The following options were not recognized by any processor: '[androidManifestFile, resourcePackageName]'
```
