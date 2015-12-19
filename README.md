# gradle_plugins
This repository collects my gradle plugins.

- provided scope plugin

## Release Note
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
