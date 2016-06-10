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
git commit -m 'x'
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

### Assignment submission

http://chara.epfl.ch/~dockermoocs/progfun1/example.zip




### Functions and Evaluation

