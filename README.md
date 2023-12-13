<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>com.ravi.cal</groupId>
   <artifactId>RaviCalculator</artifactId>
   <version>1.2-SNAPSHOT</version>
   <packaging>jar</packaging>
   <name>RaviCalculator</name>
   <url>http://maven.apache.org</url>
   <properties>
      <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
      <maven.compiler.source>1.6</maven.compiler.source>
      <maven.compiler.target>1.6</maven.compiler.target>
   </properties>
   <dependencies>
      <dependency>
         <groupId>junit</groupId>
         <artifactId>junit</artifactId>
         <version>4.8.2</version>
         <scope>test</scope>
      </dependency>
   </dependencies>
   <build>
      <plugins>
         <plugin>
            <!-- Building an executable jar -->
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-jar-plugin</artifactId>
            <version>3.1.0</version>
            <configuration>
               <archive>
                  <manifest>
                     <!-- give full qualified name of your main class-->
                     <mainClass>com.ravi.cal.RaviCalculator.Calculator</mainClass>
                  </manifest>
               </archive>
            </configuration>
         </plugin>
      </plugins>
   </build>
</project>
