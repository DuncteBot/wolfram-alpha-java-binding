Java Library for the Wolfram|Alpha API

Version 1.1

This library supports most, but not all, of the features of version 2
of the Wolfram|Alpha API.

This is not an official or supported product of Wolfram Alpha LLC. 
It is used internally for some projects, though, and it will be 
updated and maintained in the future. You are free to use and modify
this code in any way you wish, as long as it is consistent with your
license for using the Wolfram|Alpha API itself.


At the moment, there are no JavaDocs for this library, although that is
a priority for an upcoming update. In the meantime, the sample program,
along with reading the library code itself, will be your guide.
Considerably more documentation is on the way.

You need the following dependent libraries on your classpath:

     commons-codec-1.3.jar
     httpclient-4.0.1.jar
     httpcore-4.0.1.jar
     commons-logging.jar
     
These libraries are widely available on the Internet. You can probably
use other version numbers than these, although these are the versions
I used.


Look at the simple sample program included to get started.

Add this to your pom.xml to use it with maven:

<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
<dependency>
    <groupId>com.github.aeurielesn</groupId>
    <artifactId>wolfram-alpha-java-binding</artifactId>
    <version>master-SNAPSHOT</version>
</dependency>

Add this to your build.gradle to use it with gradle:

allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
dependencies {
        implementation 'com.github.aeurielesn:wolfram-alpha-java-binding:master-SNAPSHOT'
}