# Quarkus

An open-source set of technologies adapted to GraalVM and HotSpot to write Java applications. It offers (promise) a super-fast startup time and a lower memory footprint. This makes it ideal for containers and serverless workloads

GraalVM is a universal and polyglot virtual machine (JavaScript, Python, Ruby, R, Java, Scala, Kotlin). The GraalVM (specifically Substrate VM) makes possible the ahead-of-time (AOT) compilation, converting the bytecode into native machine code, resulting in a binary that can be executed natively


1. Checkout the repo and perform mvn clean install
2. cd demo (this is spring boot application)
3. To start demo application, perform below steps
```aidl
Go to demo directory
cd /demo
mvn clean package
cd /target
java -jar demo-0.0.1-SNAPSHOT.jar
Access http://localhost:8081/hello-spring

```
4. Below steps need to be perform to run quarkus application
```aidl
cd /code-with-quarkus

Use this command to run server 
./mvnw compile quarkus:dev

To run with standalone mode use below steps :

mvn clean package 
java -jar code-with-quarkus-1.0.0-SNAPSHOT-runner.jar
```

5. use jconsole to check memory leakages and classes loaded in the JVM