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
  &lt;settings&gt;
 
  &lt;profiles&gt;
    &lt;profile&gt;
      &lt;id&gt;apache-snapshots&lt;/id&gt;
      &lt;repositories&gt;
        &lt;repository&gt;
          &lt;id&gt;apache-snapshots&lt;/id&gt;
          &lt;url&gt;http://repository.apache.org/snapshots/&lt;/url&gt;
          &lt;releases&gt;
            &lt;enabled&gt;false&lt;/enabled&gt;
          &lt;/releases&gt;
          &lt;snapshots&gt;
            &lt;enabled&gt;true&lt;/enabled&gt;
          &lt;/snapshots&gt;
        &lt;/repository&gt;
      &lt;/repositories&gt;
    &lt;/profile&gt;
  &lt;/profiles&gt;
 
  &lt;activeProfiles&gt;
    &lt;activeProfile&gt;apache-snapshots&lt;/activeProfile&gt;
  &lt;/activeProfiles&gt;
&lt;/settings&gt;
</pre>

Licenses
---------

libJXR is licensed under the Apache 2.0 license.
