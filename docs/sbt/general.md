# General

## Creating a new Sbt project
___

Sbt has a command called new, to create new build definitions from a template.

To use `sbt new` you will need Sbt version 0.13.13 or above

	$ sbt sbtVersion
	> 0.13.17

To setup a new scala sbt project

	$ sbt new scala/scala-seed.g8

List of giter8 templates from official sources can be found [here](https://github.com/foundweekends/giter8/wiki/giter8-templates)

### Project sbt version
- As part of your build definition, specify the version of sbt that your build uses.
- Project will always build using the same version of Sbt, ignoring the global Sbt version.

Create a file named `project/build.properties` then specify the sbt version as follows:

	sbt.version=0.13.17

## Layout
___

???

### Shell
___

???

## Plugins
___

???
