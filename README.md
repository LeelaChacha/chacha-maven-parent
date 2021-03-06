# chacha-maven-parent
This repository contains a Parent POM for my Maven projects.

## Usage
If you want to use this POM or your own POM hosted on Github, you have to use [jitpack](https://jitpack.io/).

Jitpack acts like a Maven Repository that clones a Github Repo and buildes it and provides the result an artifact.
To declare jitpack as a repository, you can add it to your POM file.

**pom.xml**
```
<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
```
**then add the parent to the pom.xml**
```
<parent>
    <groupId>com.github.__User__</groupId>
    <artifactId>__Repo__</artifactId>
    <version>__Tag__</version>
</parent>
```

## What's Included
The following dependencies and plugins are included in release v1.2:
### Dependencies
#### General-Purpose
- lombok 1.18.20

#### Logging:
- slf4j 1.7.32

#### Testing
- junit 5.7.2
- assertj 3.20.2
- mockito 3.12.1

### Plugins
- all standard maven plugins