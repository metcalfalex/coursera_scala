# coursera_scala
Functional Programming Principles in Scala

https://www.coursera.org/learn/progfun1

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
git commit -m 'tools setup'
git push
```

## Week 1

### Getting Started

eclipse IDE  
SBT scala build tool  

Next Steps:  
1. Tools setup  
2. Practice submitting an assignment  

### Tools Setup

#### AWS EC2 for java/scala (linux)

See https://github.com/metcalfalex/quickstream > Launch server

#### Installing JDK (linux)

https://gist.github.com/tankchintan/1335220

```bash

wget --no-cookies --header "Cookie: gpw_e24=xxx; oraclelicense=accept-securebackup-cookie;" http://download.oracle.com/otn-pub/java/jdk/8u91-b14/jdk-8u91-linux-x64.rpm

sudo rpm -i jdk-8u91-linux-x64.rpm

rm jdk-8u91-linux-x64.rpm

```

#### Installing SBT (linux)

http://www.scala-sbt.org/release/docs/Setup.html

```bash
curl https://bintray.com/sbt/rpm/rpm | sudo tee /etc/yum.repos.d/bintray-sbt-rpm.repo

sudo yum install sbt

sbt about
```

#### Installing JDK (windows)

http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

#### Installing SBT (windows)


#### Installing Scala IDE for Exlipse (windows)



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

