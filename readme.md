About this project:
This is an assignment on how to use Gradle in a project. (PR16Module18)

This project demonstrates how to create a simple custom Gradle task that
accepts CLI parameters and adds external libraries using Gradle's
dependency management. The project prints a greeting message based on
the input provided from the command line.

## Features
- A custom Gradle task that accepts a `name` parameter from the CLI
  and prints a personalized greeting message.
- Adds external libraries such as Google Guava and JUnit for further
  development and testing.

## Prerequisites
Ensure you have the following installed:
- [Java JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) (version 11 or higher)
- [Gradle](https://gradle.org/install/) (version 6.8 or higher)
- Git

## Installation

To install and run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ernigee/Belajar-Gradle

2. Navigate into the project directory:
   cd <Belajar Gradle>
3. Run the Gradle task: Use the following command to run the c
   custom task and pass the name parameter:

   `Task greetingTask() {
   doLast {
   String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
   println "Hello, $nama! Welcome to Gradle World!"
   } }`

The task will print:

// Hello, YourName! Welcome to Gradle World!

## Dependencies
his project uses Gradle's dependency management to include
the following libraries:

- Guava: A set of core libraries for Java (`com.google.guava:guava:29.0-jre`).
- JUnit: A popular testing framework for Java (`junit:junit:4.13`).


To add these dependencies, the following block is added to the build.gradle file:

`dependencies {
implementation 'com.google.guava:guava:29.0-jre'
testImplementation 'junit:junit:4.13'
}`

## Pushing to GitHub
After you have created the project and added your custom task and dependencies,
you can push the project to GitHub by following these steps:

- Initialize a Git repository:
  `git init`
- Add files to the staging area:
  `git add .`
- Commit the changes:
  `git commit -m "Initial commit"`
- Add the remote repository:
  `git remote add origin https://github.com/<your_username>/<repository_name>.git`
- Push the project to GitHub:
  `git push -u origin master`

## Objective
The objective of this assignment is to create a custom Gradle task that demonstrates how Gradle can handle CLI parameters, as well as how to manage dependencies using Gradle.
