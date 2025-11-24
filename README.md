# Health & Diet Analyzer for Hostel Students (Java)

**Student:** GAURAV BHARDWAJ  
**Reg:** 24BSA10187

This is a Java console application skeleton for the course project "Health & Diet Analyzer for Hostel Students."

## What is included
- A simple Maven-like Java project structure under `src/`
- Core Java classes for Users, FoodItems, Meals, Nutrition aggregation, and a basic JSON-based datastore
- Sample data files in `data/`
- `pom.xml` for reference (no external dependencies)
- Scripts to compile and run with `javac` and `java`

## How to compile & run (Linux / macOS / Windows with Git Bash)
1. Open the terminal in the project root.
2. Compile:
   ```
   javac -d out $(find src -name "*.java")
   ```
   (On Windows, use PowerShell or change the find command.)
3. Run:
   ```
   java -cp out com.healthdiet.Main
   ```
4. The app displays a console menu to add meals and view today's summary.

## Maven usage (recommended)
This project is set up as a Maven project. To build and run:

1. Make sure Maven and Java 17 or newer are installed.
2. From the project root:
   - `mvn clean compile`
   - `mvn exec:java -Dexec.mainClass=com.healthdiet.Main`

To run tests:
   - `mvn test`

You can also run `./run.sh` (Unix) or `run.bat` (Windows) to compile and execute.
