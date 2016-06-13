# coursera_scala
Functional Programming Principles in Scala

https://www.coursera.org/learn/progfun1

http://www.tryscala.com/

## Week 0

### Google: Scala Tutorial

http://www.tutorialspoint.com/scala/  
http://www.scala-lang.org/documentation/  
https://twitter.github.io/scala_school/  
http://blog.codacy.com/2015/07/03/how-to-learn-scala/#gs.ACTcS44  
http://joelabrahamsson.com/learning-scala/  

### Update Git

```bash
cd /c/git/coursera_scala
git add README.md
git commit -m 'wk01 video notes'
git push
```

## Week 1

### Getting Started

eclipse IDE  
SBT scala build tool  

Next Steps:  
1. Tools setup  
2. Practice submitting an assignment  

### Tools Setup (linux)

#### AWS EC2 for java/scala

See https://github.com/metcalfalex/quickstream > Launch server

#### Installing JDK

https://gist.github.com/tankchintan/1335220

```bash

wget --no-cookies --header "Cookie: gpw_e24=xxx; oraclelicense=accept-securebackup-cookie;" http://download.oracle.com/otn-pub/java/jdk/8u91-b14/jdk-8u91-linux-x64.rpm

sudo rpm -i jdk-8u91-linux-x64.rpm

rm jdk-8u91-linux-x64.rpm

```

#### Installing SBT

http://www.scala-sbt.org/release/docs/Setup.html

```bash
curl https://bintray.com/sbt/rpm/rpm | sudo tee /etc/yum.repos.d/bintray-sbt-rpm.repo

sudo yum install sbt

sbt about
```

### Tools Setup (windows)

#### Installing JDK

http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

#### Installing SBT

http://www.scala-sbt.org/

#### Installing Scala IDE for Exlipse (windows)

http://scala-ide.org/download/sdk.html

#### Installing Scala SBT plugin

If it doesn't already exist, create the following folder/file:  
C:\Users\metcaal\.sbt\0.13\plugins\plugins.sbt

Place the following statement into pluginst.sbt:  
```
addSbtPlugin("com.typesafe.sbteclipse" % "sbteclipse-plugin" % "4.0.0")
```

Run sbt from windows command line.  
if set up correctly, sbt should download JAR files required for plugin.

### Assignment submission

```bash
mkdir wk01
cd wk01
wget http://chara.epfl.ch/~dockermoocs/progfun1/example.zip
unzip example.zip
```

Interpreter = REPL = read, eval, print, loop

```bash
sbt
console
println("hello hello")
val l = List(1, 2, 3)
val squares = l.map(x => x * x)
```

ctrl-d exists scala repl  
ctrl-c exists sbt shell  







### Functions and Evaluation

Call by Name: only call required parameters  
Call by Value: evaluate all parameters regardless of whether required

Default is CBV  
Use => to force CBN

def: cbn  
val: cbv (on definition)

```scala
// attempt 1:  
def and(x:Boolean, y:Boolean): Boolean = {if (x) {if (y) {true}else{false}}else{false}}

// attempt 2:
def and(x: => Boolean, y: => Boolean) = if (x) {if (y) true else false} else false
and(true,true)
```

ctrl-shift-f: auto format

```scala
def sqrIter(guess: Double, x: Double): Double = {
	if (isGoodEnough(guess,x)) guess
	else sqrtIter(improve(guess, x), x)
}

```
