# Repository for Project functions-starter

## Maven instructions

The repository is configured with maven to retrieve all necessary dependencies, as well as to run automatically the parsing classes on build.  If you do not know how to use maven, please look at [this tutorial](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html). Follow the following instructions:

    git clone git@github.com:ubc-cpsc411-2016w2/functions-starter.git
	cd functions-starter/
	mvn clean dependency:copy-dependencies
	mvn test
	
And voila! You have run your tests.  Maven should recompile your code every time you run `mvn test`.

## Instructions on how to add JavaCC as an external tool in IntelliJ IDEA

This instructions will help you to add a menu option to run JavaCC as to generate the Parser whenever you make changes to the ExpressionParser.jj file.

### Setup
Go to Preferences > Tools > External Tools > + and fill up the Dialog as follows:

![Setup of JavaCC](adding_javacc_1.png)

### Use
Right-click on the ExpressionParser.jj file and click the JavaCC button in the External Tools menu, as follows:

![Use of JavaCC](adding_javacc_2.png)

Or, alternatively, choose Tools > External Tools > JavaCC in the Menu Bar when you are editing the ExpressionParser.jj file.

