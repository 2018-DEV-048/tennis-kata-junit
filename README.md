# tennis-kata-junit
Below are the steps to run tennis-kata-junit application on windows OS.

1) If java not installed on local machine follow below steps:-

	a) download latest java version from below link:-
	
	https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
	
	b) go to System Properties --> Environment Variables. create new System variable as JAVA_HOME and set path "C:\Program Files (x86)\Java\jdk1.8.0_91\" (the path where java stored in local machine)
	
	c) go to System Properties --> Environment Variables, edit 'Path' environment variable by adding "%JAVA_HOME%\bin" into it.
	
	d) open command prompt and run java -version, it will give below like output. This is the confirmation that java is installed and running properly.
	
		java version "1.8.0_121"
		Java(TM) SE Runtime Environment (build 1.8.0_121-b13)
		Java HotSpot(TM) 64-Bit Server VM (build 25.121-b13, mixed mode)
		

		
3) If maven not install on local machine follow below steps:-

	a) Download maven from below location.
	
	https://maven.apache.org/download.cgi
	
	b) Go to System Properties --> Environment Variables. create new System variable as MAVEN_HOME and set path "....\apache-maven-3.0.5-bin\apache-maven-3.0.5" (the path where maven stored in local machine)
	
	b) Go to System Properties --> Environment Variables. create new System variable as M2_HOME and set path "....\apache-maven-3.0.5-bin\apache-maven-3.0.5" (the path where maven stored in local machine)
	
	c) Go to System Properties --> Environment Variables, edit 'Path' environment variable by adding "%M2_HOME%\bin" and "%MAVEN_HOME%\bin" into it.
	
	d) Open command prompt and run mvn -version, it will give below like output. This is the confirmation that maven is installed and running properly.
	
		Apache Maven 3.0.5 (r01de14724cdef164cd33c7c8c2fe155faf9602da; 2013-02-19 19:21:28+0530)
		Maven home: D:\Softwares\apache-maven-3.0.5-bin\apache-maven-3.0.5
		Java version: 1.8.0_91, vendor: Oracle Corporation
		Java home: C:\Program Files (x86)\Java\jdk1.8.0_91\jre
		Default locale: en_US, platform encoding: Cp1252
		OS name: "windows 10", version: "10.0", arch: "x86", family: "dos"
		
4) Click on "Download ZIP" button on GitHub, it will download "tennis-kata-junit-master.zip" folder. Unzip it and open it.
5) Open command prompt, Go to inside tennis-kata-ui-master/tennis-kata-junit/ folder.
6) run 'mvn clean' command to clean the project.
7) Run 'mvn test' command to run junit test cases.
8) Go to tennis-kata-junit-master\tennis-kata-junit\target\surefire-reports\ folder
9) Can see test reports in xml format.
10) If want to build project and want to create its jar file then Open command prompt, Go to inside tennis-kata-ui-master/tennis-kata-junit/ folder.
11) Run 'mvn install' command to build project.
12) tennis-kata-junit.jar will be created inside tennis-kata-ui-master/tennis-kata/target/ folder.
