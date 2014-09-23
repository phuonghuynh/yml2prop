yml2prop
========

This is a Maven Plugin which helps to generate *.properties from *.yaml (www.yaml.org).

Welcome to the yml2prop wiki!

It is quiet simple, as bellow:
<plugin>
   <groupId>org.apache.maven.plugins</groupId>
   <artifactId>yml2prop</artifactId>
   <configuration>
      <sourceYaml>${basedir}/src/main/resources/test.yml</sourceYaml>
      <entries>
         <param>dev</param>
         <param>prod</param>
      </entries>
   </configuration>
   <executions>
      <execution>
         <phase>generate-resources</phase>
         <goals>
            <goal>run</goal>
         </goals>
      </execution>
   </executions>
</plugin>

Configuration params:
* sourceYaml: String - source path of your yaml file
* entries: Array of Strings - array of names that will be used to extracted to *.properties, ex: dev, prod, staging...
* destProp: String - destination path of your properties file
