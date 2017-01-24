# Repository for Functions language compiler project

The repository is configured with maven to retrieve all necessary dependencies, as well as to run automatically the parsing classes on build.

## Instructions to start working on IntelliJ IDEA
You can find detailed instructions on how to setup IntelliJ with Github at https://www.jetbrains.com/help/idea/2016.3/using-github-integration.html

Once you have setup IntelliJ IDEA to work with Github:

- Open the Clone Repository dialog. To do so, either:
  - Go to File -> New -> Project from Version Control -> Github
  - Click "Check out from Version Control" -> Github on the "Welcome to IntelliJ IDEA" dialog
- Fill Git Repository URL with https://github.com/ubc-cpsc411-2016w2/functions-starter.git
- Click Clone
- Done

### Maven Integration
	
We use Maven in the IntelliJ IDEA IDE to automatically run the JavaCC parser generator before builds.  You can also run any maven goals from IntelliJ if you so desire.

## Console instructions

The repository is configured with maven to retrieve all necessary dependencies, as well as to run automatically the parsing classes on build.  If you do not know how to use maven, please look at [this tutorial](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html).  Once you have installed maven on your machine, follow the following instructions (if you have setup an SSH key with github.  Otherwise, replace the `git clone` line with the correct URL):

    git clone git@github.com:ubc-cpsc411-2016w2/functions-starter.git
	cd functions-starter/
	mvn clean dependency:copy-dependencies
	mvn test
	
And voila! You have run your tests.  Maven should recompile your code every time you run `mvn test` if there are any changes.

