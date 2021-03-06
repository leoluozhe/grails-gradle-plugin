# Change Log

## v2.1.0

## v2.0.1

+ Fix a bug in setting `grails.groovyVersion` which resulted in an exception when a dependency tried to include the
  `groovy` library.
+ Fix a bug where when a GrailsTestTask is configured with both a set of Task Inputs and a `testResultsDir` that
  results in an exception because `testResultsDir` is a directory but Gradle expects it to be a file.
+ Fix a bug in the task dependency configuration for the `clean` task that results in Gradle being unabled to determine
  the task graph.
+ Add plugin Zip file or application War file as an output file to the runtime configuration.
+ Configured the default configuration to extend from runtime (similar to Java plugin behavior)
+ Springloaded is only configured for the 'grails-run-app' task (this is what Grails itself does in grailsStart).
+ Added the 'init-plugin' task to initialize a Grails plugin instead of an application.
+ The 'grails-run-app' task is now available on plugin projects as well (Grails allows this)