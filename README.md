# Task08: Simple Java Maven Build with Jenkins 🚀

## Objective
Learn how to use Jenkins to build a simple Java application using Maven — your first step into CI/CD.

---

## Tools Required
- Jenkins (locally or via Docker)
- Java JDK 8 or 11
- Maven
- Git

---

## Folder Structure

Task08/ <-- Root folder

├── pom.xml <-- Maven build file

└── src/

└── main/

└── java/

└── HelloWorld.java

---


## Files Description
1. **HelloWorld.java**  
   Prints `Hello, Jenkins + Maven!` to the console.

2. **pom.xml**  
   Maven configuration file specifying Java version and build plugins.

---

## Jenkins Build

1. Start Jenkins (Docker or local)

2. Install Maven in Global Tool Configuration

3. Create a Freestyle Project → Name: Hello-Java-Maven

4. Set Source Code Management → Git → https://github.com/vishakhachachare/Task08.git

5. Build section → Invoke top-level Maven targets → Goal: clean package

Save & Build

Check Console Output → You should see:

```
[INFO] BUILD SUCCESS
```

---

Notes

Java and Maven are pre-configured on this setup ✅

Make sure Jenkins has Git installed if you want SCM integration.

Default package is used in HelloWorld.java to avoid compilation issues in Jenkins.
