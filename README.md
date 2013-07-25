libJXR - a fork of maven-jxr
======================================== 

libJXR is a fork of [maven-jxr](http://maven.apache.org/jxr/) with the following extra features:
  
 * Optional footer (and ability to set one)
 * Formating fixes in the **&lt;pre&gt;** tag
 * Lines are now inside of **&lt;div&gt;** for easier manipulation
 * Default output encoding is now UTF-8

Usage
--------

Usage is the same as the maven-jxr, so the tutorial at [maven-jxr usage](http://maven.apache.org/jxr/examples/java.html)
applies.

Build
---------

In order to build the project you need the apache snapshot repository enabled in your ~/.m2/settings.xml.
To do that you need to add the following to that file:
  <pre>
  <settings>
 
  <profiles>
    <profile>
      <id>apache-snapshots</id>
      <repositories>
        <repository>
          <id>apache-snapshots</id>
          <url>http://repository.apache.org/snapshots/</url>
          <releases>
            <enabled>false</enabled>
          </releases>
          <snapshots>
            <enabled>true</enabled>
          </snapshots>
        </repository>
      </repositories>
    </profile>
  </profiles>
 
  <activeProfiles>
    <activeProfile>apache-snapshots</activeProfile>
  </activeProfiles>
</settings>
</pre>

Licenses
---------

libJXR is mostly Apache 2.0 with the parts modified by me being MIT.
