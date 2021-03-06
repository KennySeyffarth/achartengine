# What is it?
The code in the repository is a fork of [achartengine][homepage] at [google code][source].
I just added a pom to build the jar with maven to consume the artifacts in an android project I build with maven too.
[source]:http://code.google.com/p/achartengine/
[homepage]:http://www.achartengine.org

# Why I did it
The oldest still unresolved [tickets][ticket] in the chartengine issue tracker is to provide a maven artifacts for others to consume.
One of the [comments][comment] points to [another mavenized fork][old fork] to build the library.
For me there where some problems:  

1. it is not up to date  
2. it produces an apklib instead of a jar like the offical release

[ticket]: http://code.google.com/p/achartengine/issues/detail?id=4
[comment]: http://code.google.com/p/achartengine/issues/detail?id=4#c14
[old fork]: https://github.com/jondwillis/AChartEngine

# How can anyone use it?
1. clone this repository
2. *cd achartengine/trunk/achartengine/*
3. *mvn clean install*
4. add the dependency in to your projects pom

```xml
    <dependency>
        <groupId>org.achartengine</groupId>
        <artifactId>achartengine</artifactId>
        <version>1.0.0-r452</version>
    </dependency>
```

The [qualifier][maven-version-scheme] behind the version number is the svn repository version of the current code in the git repository.
Right now I only build the library. I do not build the demo that is provided on google code.

[maven-version-scheme]:http://mojo.codehaus.org/versions-maven-plugin/version-rules.html


# Any issues with achartengine?
I am not the developer of achartengine.
To contact the developers of achartengine please use the [issue-tracker][google-code-tracker] at google code to file bug reports, feature requests or any other feedback directly relating to achartengine.

If the code on [google-code][source] changes and I have not merged it into this repository please create an [issue][my issue tracker] or send me a pull request.
[my issue tracker]:https://github.com/signed/achartengine/issues
[google-code-tracker]:http://code.google.com/p/achartengine/issues/list