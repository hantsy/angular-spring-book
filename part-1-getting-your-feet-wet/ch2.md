# Setup local development environment

Before writing any codes, you have  to prepare the development environment in your local system.  The backend APIs is built with Spring Boot,  so you should prepare a Java development environment.



## Tools for backend development

 Firstly you should get a OpenJDK redistribution installed in your system. 

### Java 11

According to [the latest Java trends report](https://www.jetbrains.com/lp/devecosystem-2019/jav) from Jetbrains, currently the most widely-used Java version is Java 8, next is Java 11. 

After Java 9, Oracle had changed Java release progress and tried to speed up the Java releases in very six months .   And the next long term support version is  Java 11, which is recommended to use in commercial products. 

Oracle had ended security updates of Java 8 in the early 2019.  In this book, we will use Java 11  as Java development environment. Aligned with Spring Boot 2.2, we will try to use the latest  Java language feature from Java 8 to Java 11.  

You can download one of the following JDK 11 redistribution, and get it installed into your system.

* [The official OpenJDK 11](http://openjdk.java.net/)
* [Oracle  JDK 11](https://java.oracle.com)
* [Redhat OpenJDK redistribution](https://developers.redhat.com)
* [AdoptOpenJDK  redistribution](https://adoptopenjdk.net/)

Additionally, [Azul](https://www.azul.com/downloads/zulu-community/),  [Amazon](https://aws.amazon.com/corretto/),  [Alibaba](https://github.com/alibaba/dragonwell8),  and [Microsoft](https://docs.microsoft.com/en-us/xamarin/android/get-started/installation/openjdk)  have maintained their own OpenJDK redistribution for their products. 

I prefer AdoptOpenJDK,  because AdoptOpenJDK is maintained by Java communities.

Optionally, you can set **JAVA\_HOME** environment variable and add *&lt;JDK installation dir>/bin* in your **PATH** environment variable.

Open your terminal, execute the following command to verify your Java environment installed successfully.

```sh
#java -version
openjdk version "11.0.4" 2019-07-16
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.4+11)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.4+11, mixed mode)
```

### Apache Maven

Apache Maven and Gradle are the most popular build tools in the Java communities. 

Personally, I prefer Apache Maven.  

Download the latest Apache Maven from [http://maven.apache.org](http://maven.apache.org), and extract the files into your local system. 

Optionally, you can set **M2\_HOME** environment variable, and also do not forget to append *&lt;Maven Installation dir>/bin* your **PATH** environment variable.  

Type the following command to verify Apache Maven is working.

```shell
#mvn -v
Apache Maven 3.6.1 (d66c9c0b3152b2e69ee9bac180bb8fcc8e6af555; 2019-04-05T03:00:29+08:00)
Maven home: D:\build\maven\bin\..
Java version: 11.0.4, vendor: AdoptOpenJDK, runtime: D:\jdk11
Default locale: en_US, platform encoding: Cp1252
OS name: "windows 10", version: "10.0", arch: "amd64", family: "windows"
```



###  Gradle (Optional)

If you are a Gradle fan, get it from [Gradle website](https://gradle.org/), and [install](https://gradle.org/install) it into your system.

```sh
gradle -v

Welcome to Gradle 5.5.1!

Here are the highlights of this release:
 - Kickstart Gradle plugin development with gradle init
 - Distribute organization-wide Gradle properties in custom Gradle distributions
 - Transform dependency artifacts on resolution

For more details see https://docs.gradle.org/5.5.1/release-notes.html


------------------------------------------------------------
Gradle 5.5.1
------------------------------------------------------------

Build time:   2019-07-10 20:38:12 UTC
Revision:     3245f748c7061472da4dc184991919810f7935a5

Kotlin:       1.3.31
Groovy:       2.5.4
Ant:          Apache Ant(TM) version 1.9.14 compiled on March 12 2019
JVM:          11.0.4 (AdoptOpenJDK 11.0.4+11)
OS:           Windows 10 10.0 amd64
```

### Java IDE 

The most popular integration development environment in Java communities includes:

* The most popular Java IDE is [Intellij IDEA from Jetbrains](https://www.jetbrains.com/idea/) .  The free and open-source community edition includes basic language supports for Java, Kotlin, Groovy, etc..  If you want to get [more features](https://www.jetbrains.com/idea/features/editions_comparison_matrix.html), buy a commercial license of the ultimate edition. 
* The refactored [Spring Tools 4](https://spring.io/tools)   supports Eclipse, [VS Code](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-boot-dev-pack), [Eclipse Theia](https://github.com/theia-ide/theia), get it from [Spring website](https://spring.io/tools).
* Apache NetBeans have just graduated from Apache incubator, it is still a  great Java IDE. To get better   Spring Boot support , install [NbSpringBoot](http://plugins.netbeans.org/plugin/67888/nb-springboot) plugin from NetBeans plugin portal please.

You can choose your favorite one to write Java codes.

## Tools for frontend development



NodeJS is a Javascript runtime built on [Chrome's V;8 Javascript engine](https://v8.dev/).  It was initially designated for backend Javascript development, but it is very popular in the frontend development. 

### NodeJS

Get the latest NodeJS from [NodeJS website](https://nodejs.org), and install it into your local system.

```sh
#node -v
v12.7.0
```

The most attractive feature of NodeJS is its package management, aka NPM. Nowadays,  most of the popular Javascript projects are published via NPM registry,  which is a central place to share your Javascript package to others.   The NPM client tool is shipped with NodeJS installation by default.

```sh
>npm -v
6.10.0
```

Another popular packager is [Yarn](https://yarnpkg.com/en), which is created by Facebook.  Please go to the yarn website to get more details.

### VS Code 

As a sibling project of Visual Studio,  VS Code provides a lightweight code environment for web developers. 

Get a copy of VSCode from [VS Code website](https://code.visualstudio.com), and install it into your system.  To improve Angular code experience, you can install some useful extensions from  VSCode marketplace, eg.  The [Angular Essentials](https://marketplace.visualstudio.com/items?itemName=johnpapa.angular-essentials) extension pack  includes several popular plugins which is helpful to build an  Angular application. 











