# roomtogo
selenium/java/appium/xcode-simulator/


pre-requisite requirements 

install java - make sure to use java 1.5 
java ( configure java to the path - mac : export JAVA_HOME=/Library/Java/Home )  

                                windows : set path=C:\Program Files\Java\jdk1.6.0_23\bin

                                  
xcode ( version 7.3 ) strictly use 7.3 because there is compability issue between new xcode version and appium version ( 1.6.2)

xcode - setup for simulator 
         - download xcode 7.3 
         - after installing 
         - click xcode from the menu 
         - open developer tools 
         - simulator ( by default it will start with a newest iphone simulator device ) 
         - click on hardware menu - device - ios 9.3 - iphone 6 simulator 

appium desktop ( version 1.6.2 ) launch the server from default port just start it 

Mac - OS high Sierra( 10.13.6 )  chose any OS 

eclipse ( photon 4.8.0 ) use whatever you like 

maven - add this jar to your pom.xml 
      - selenium server jar ( this sud download all the dependency for any broweser and any language ) 
      - selenium remote driver jar ( for desiredcapabilities dependency ) 
      - testng jar ( for testing ) a unit testing framework 
      - appium java client jar - simply appium/java language binding ( provides extra api methods - such as ( IOSDriver ) 
      
      <dependencies>

		<!-- https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-server -->
		<dependency>
			<groupId>org.seleniumhq.selenium</groupId>
			<artifactId>selenium-server</artifactId>
			<version>3.14.0</version>
		</dependency>

		<!-- https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-remote-driver -->
		<dependency>
			<groupId>org.seleniumhq.selenium</groupId>
			<artifactId>selenium-remote-driver</artifactId>
			<version>3.14.0</version>
		</dependency>

		<!-- https://mvnrepository.com/artifact/org.testng/testng -->
		<dependency>
			<groupId>org.testng</groupId>
			<artifactId>testng</artifactId>
			<version>6.14.3</version>
			<scope>test</scope>
		</dependency>

		<!-- https://mvnrepository.com/artifact/io.appium/java-client -->
		<dependency>
			<groupId>io.appium</groupId>
			<artifactId>java-client</artifactId>
			<version>6.1.0</version>
		</dependency>

	</dependencies>
