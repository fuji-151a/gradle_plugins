# gradle_plugins
This repository collects my gradle plugins.
## Plugin List

- provided scope plugin
- integrationTest plugin

## Release Note
- **1.1.0**  
  create integrationTest plugin
- **1.0.0**  
  create provided plugin

## provided scope plugin
This plugin adds 'provided scope'
### How to Use
import this plugin.  
write build.gradle

```
apply: 'https://raw.githubusercontent.com/fuji-151a/gradle_plugins/master/provided.gradle
```
or
```
apply: 'https://raw.githubusercontent.com/fuji-151a/gradle_plugins/<release tag>/provided.gradle
```

For example
```
dependencise {
  provided 'org.apache.storm:storm-core:0.9.5'
}
```

## integrationTest plugin
This plugin adds integration testing task to Gradle projects.
### How to use
import 
```
apply: 'https://raw.githubusercontent.com/fuji-151a/gradle_plugins/master/integrationTest.gradle
```
or
```
apply: 'https://raw.githubusercontent.com/fuji-151a/gradle_plugins/<release tag>/integrationTest.gradle
```
For example:)  
add dependencies of test framework.  
```
dependencies {
    integrationTestCompile 'junit:junit:4.12'
}
```
run gradle task.  
This plugin set to target *IT and *Test class file.  
```
$ gradle integrationTest
```