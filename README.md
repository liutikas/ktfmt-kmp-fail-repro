# Reproduction case for ktfmt-gradle failure for KMP

## Steps

1. `./gradlew ktfmtFormat`


## Expected

It works!

## Actual

```
* What went wrong:
Some problems were found with the configuration of task ':lib:ktfmtFormatKmpAndroidAndroidTest' (type 'KtfmtFormatTask').
  - Gradle detected a problem with the following location: '/ssd/ssd1/temp/KmpKtfmt/lib/src/androidAndroidTest/kotlin'.
    
    Reason: Task ':lib:ktfmtFormatAndroidTest' uses this output of task ':lib:ktfmtFormatKmpAndroidAndroidTest' without declaring an explicit or implicit dependency. This can lead to incorrect results being produced, depending on what order the tasks are executed.
    
    Possible solutions:
      1. Declare task ':lib:ktfmtFormatKmpAndroidAndroidTest' as an input of ':lib:ktfmtFormatAndroidTest'.
      2. Declare an explicit dependency on ':lib:ktfmtFormatKmpAndroidAndroidTest' from ':lib:ktfmtFormatAndroidTest' using Task#dependsOn.
      3. Declare an explicit dependency on ':lib:ktfmtFormatKmpAndroidAndroidTest' from ':lib:ktfmtFormatAndroidTest' using Task#mustRunAfter.
    
    Please refer to https://docs.gradle.org/8.0/userguide/validation_problems.html#implicit_dependency for more details about this problem.
  - Gradle detected a problem with the following location: '/ssd/ssd1/temp/KmpKtfmt/lib/src/androidTest/java'.
    
    Reason: Task ':lib:ktfmtFormatAndroidTest' uses this output of task ':lib:ktfmtFormatKmpAndroidAndroidTest' without declaring an explicit or implicit dependency. This can lead to incorrect results being produced, depending on what order the tasks are executed.
    
    Possible solutions:
      1. Declare task ':lib:ktfmtFormatKmpAndroidAndroidTest' as an input of ':lib:ktfmtFormatAndroidTest'.
      2. Declare an explicit dependency on ':lib:ktfmtFormatKmpAndroidAndroidTest' from ':lib:ktfmtFormatAndroidTest' using Task#dependsOn.
      3. Declare an explicit dependency on ':lib:ktfmtFormatKmpAndroidAndroidTest' from ':lib:ktfmtFormatAndroidTest' using Task#mustRunAfter.
    
    Please refer to https://docs.gradle.org/8.0/userguide/validation_problems.html#implicit_dependency for more details about this problem.
  - Gradle detected a problem with the following location: '/ssd/ssd1/temp/KmpKtfmt/lib/src/androidAndroidTest/kotlin'.
    
    Reason: Task ':lib:ktfmtFormatKmpAndroidAndroidTest' uses this output of task ':lib:ktfmtFormatAndroidTest' without declaring an explicit or implicit dependency. This can lead to incorrect results being produced, depending on what order the tasks are executed.
    
    Possible solutions:
      1. Declare task ':lib:ktfmtFormatAndroidTest' as an input of ':lib:ktfmtFormatKmpAndroidAndroidTest'.
      2. Declare an explicit dependency on ':lib:ktfmtFormatAndroidTest' from ':lib:ktfmtFormatKmpAndroidAndroidTest' using Task#dependsOn.
      3. Declare an explicit dependency on ':lib:ktfmtFormatAndroidTest' from ':lib:ktfmtFormatKmpAndroidAndroidTest' using Task#mustRunAfter.
    
    Please refer to https://docs.gradle.org/8.0/userguide/validation_problems.html#implicit_dependency for more details about this problem.
  - Gradle detected a problem with the following location: '/ssd/ssd1/temp/KmpKtfmt/lib/src/androidTest/java'.
    
    Reason: Task ':lib:ktfmtFormatKmpAndroidAndroidTest' uses this output of task ':lib:ktfmtFormatAndroidTest' without declaring an explicit or implicit dependency. This can lead to incorrect results being produced, depending on what order the tasks are executed.
    
    Possible solutions:
      1. Declare task ':lib:ktfmtFormatAndroidTest' as an input of ':lib:ktfmtFormatKmpAndroidAndroidTest'.
      2. Declare an explicit dependency on ':lib:ktfmtFormatAndroidTest' from ':lib:ktfmtFormatKmpAndroidAndroidTest' using Task#dependsOn.
      3. Declare an explicit dependency on ':lib:ktfmtFormatAndroidTest' from ':lib:ktfmtFormatKmpAndroidAndroidTest' using Task#mustRunAfter.
    
    Please refer to https://docs.gradle.org/8.0/userguide/validation_problems.html#implicit_dependency for more details about this problem.

```
