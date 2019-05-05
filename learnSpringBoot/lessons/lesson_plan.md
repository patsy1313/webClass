## Spring Boot / Maven / Java Lesson Plan


### Assumptions
* You have installed Java JDK 1.8
* You have installed Maven 3.3.9
* You have installed IntelliJ<br/>
  [Setup Development Env for Unix](/learnSpringBoot/lessons/lesson01a_setupDevelopmentEnvForUnix.txt )<br>
  [Setup Development Env for Windows](/learnSpringBoot/lessons/lesson01b_setupDevelopmentEnvForWindows.txt)<br>  <br> 
  

### Lesson Plan
1. Java fundamentals<br/>
    [Exercise: Create a simple command-line Java program in Intellij](/learnJava/howToCreateJavaCommandLineProgramUsingIntellijMaven.txt)
    
1. Maven fundamentals<br/>
    Exercise: Add logback to thee command-line Java program

1. Spring fundamentals
   1. Lifecycle:  Constructor, Injection, Post-Construct
   1. Application Context / Spring beans (how does Spring manage them)
   1. Exercise: Adjust existing CDE webapp and inject code

1. Build SpringBoot webapp w/simple REST call
   1. [Build Spring Boot Structure](/learnSpringBoot/lessons/lesson02_createProjectStructure.txt)<br/>
   1. [Setup Springboot as Runnable JAR](/learnSpringBoot/lessons/lesson03_setupRunnableJar.txt)<br/>

1. Add a REST endpoint (controller)<br/>
   1. [Setup NPM](/learnSpringBoot/lessons/lesson04_addAngularUsingNpm.txt)<br/>
   1. [Add Angular Page](/learnSpringBoot/lessons/lesson05_addSimpleAngularPage.txt)<br/>
   1. [Setup Front End Structure](/learnSpringBoot/lessons/lesson06_addAngularFrontEndStructure.txt)<br/>   

1. [Setup Local Git Repo](/learnGit/howToAddProjectToLocalRepo.txt)
   
1. Add a REST endpoint that queries the database<br/>
   1. [Setup Postgres Database](/learnSpringBoot/lessons/lesson07_setupPostgresDatabase.txt)<br/>
   1. [Add JDBC Connection Pool](/learnSpringBoot/lessons/lesson09_addJdbcConnectionPool.txt)<br/>
   1. [Add REST controller, service layer, SQL call](/learnSpringBoot/lessons/lesson10_AddRestEndPoint.txt)<br/>

1. Use Flyway to setup a database table and sequence<br/>
   1. [Setup Flyway](/learnSpringBoot/lessons/lesson08a_addFlyway.txt)<br/>
   1. [Use Flyway to add database tables](/learnSpringBoot/lessons/lesson08c_useFlywayToAddTables.txt)<br/>
   1. [Use Intellij Database Plugin to run SQL](/learnIntellij/howToRunSqlInIntellij.txt)<br/>
   
1. Quick Start: Run SQL call in Java w/Spring-JDBC
   1. [Run SQL to select, insert, and delete records](/learnSpringBoot/lessons/lesson12_runSqlToInsertRecords.txt)
   1. [Create a command-line java program to run SQL call w/Spring-JDBC](/learnJdbcConnectionPools/postgreSQL/howToSetupSingleConnectionDataSourceWithIntellij.txt)
   1. [Add a Java service class to run SQL call w/Spring-JDBC](/learnSpringBoot/lessons/lesson13_addServiceLayerThatRunsSql.txt)
   1. Add bind parameters to java SQL call
  
1. Learn Advanced SQL
   1. Run SQL to join tables
   1. Run SQL to aggregate values (group by SQL)
   1. Working with database views
   1. Working with database materialized views
   
1. Working with Java collections
   1. Working with lists
   1. Working with maps
   
1. Run SQL code in Java w/Spring-JDBC
   1. Run Java code to get next value from a sequence
   1. Run Java code to run SQL update and delete calls
   1. Run Java code to run SQL insert and return newly-created id
  
1. Run SQL transactions in Java w/Spring-JDBC
   1. Run SQL transaction manually (inside & outside perspectives)
   1. Run Java code to execute a transaction 
   1. Run Java code to execute a transaction that returns an object
   
1. Create a REST endpoint that returns a list of data
   1. Construct SQL join that retrieves the data
   1. Create Java model object
   1. Create Service class to run SQL call, return list of objects
   1. Create Controller class with REST endpoint
   1. Add Angular front-end call
   
1. Creating unit tests w/JUnit
   1. Create a test case for the service class
   1. Create a test case for the controller class
   
1. Create a REST endpoint that returns a file

1. Create a REST endpoint that returns CSV values

1. Working with REST endpoint parameters
   1. How to handle optional parameters
   1. How to handle date fields

1. Handling Java Exceptions
   1. What happens when controller method throws an exception?
   1. How to gracefully handle exceptions in a controller   
   1. Setup a generic Exception handler to log all errors 
   1. Create your own "404 not found" page template -- e.g., 404.html file
   
1. Learn Java thread safety
   1. What is Thread safety?
   1. [Are my controllers and service classes thread safe?](/learnSpringBoot/lessons/lesson21_threadSafety.txt)

1. Using Spring Profiles
   1. How to setup multiple profiles in application.yaml -- e.g., "dev", "prod"
   1. How to switch profiles

1. More Maven Tricks
   1. Setup a maven profile that will replace logback.xml and application.yaml with different files (for production)
   1. Tell maven to run "npm install" when running npm clean install
   1. Tell maven to include the build-user, build-time, jenkins build name into the manifest uber jar

1. How to Create an "About" Page that displays the MANIFEST.MF
   1. Adjust Maven to create a manifest.txt
   1. Add REST call that returns the contents of manifest.txt
   1. Add page call to forward to manifest.htm
   1. Create manifest.htm page that invokes the REST call
   
1. Encoding Passwords w/Jasypt<br/>
   [Excercise: Encode database password](/learnSpringBoot/howToUseJasyptToEncode.txt)

1. Run Java code after your web app has started
   1. Used to run health checks
   
1. Add SSL and PKI Client Certificate Authentication
   1. [Setup your own Certificate Authority](/learnSSL/howToUseYourCertAuthority_InitialSetup.txt)
   1. [Create your own server certificate](/learnSSL/howToUseYourCertAuthority_MakeServerCert.txt)
   1. [Create your own PKI client certificate](/learnSSL/howToUseYourCertAuthority_MakeServerCert.txt)
   1. Configure SpringBoot to use your server cert
   1. Configure SpringBoot to require PKI client certificate
   1. Configure Security to protect your REST endpoints
   
1. Building & Deployment
   1. Create Jenkins Job to build the uber JAR
   1. Add a MANIFEST.MF to your uber JAR
   1. Read the contents of the MANIFEST.MF from command-line
   1. Create a web page that displays the contents of MANIFEST.MF