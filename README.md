yml2prop
========

This is a Maven Plugin which helps to generate *.properties from *.yaml (www.yaml.org).

Configuration parameters:
   `sourceYaml`: String - source path of your yaml file
   `entries`: Array of Strings - array of names that will be used to extracted to *.properties, ex: dev, prod, staging...
   `destProp`: String - destination path of your properties file

To run this plugin: mvn yml2prop:run
