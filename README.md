# 2017-TranspSaude
Assignment for the 2017 edition of the "Web Development and the Semantic Web" course, by Fabio da Costa Pinto and Sirhan Bortolini
This is a preliminary system to practice Web Development in Java skills, built using [JButler Framework](https://github.com/dwws-ufes/jbutler). The system intends to be a plataform to evaluate investments in health care, .
 
# Requisites
TranspSaude was built using [Eclipse Neon 3](http://www.eclipse.org/neon/) IDE and runs over [Wild Fly 10](http://wildfly.org/). Also, it is configured to connect to a [MySQL Database](https://www.mysql.com/).
 
# Configuration
The database connection is configured at WildFly configuration file `standalone.xml`. It can be edited to specify other datasource, if necessary.
 
xml
<datasource jta="true" jndi-name="java:jboss/datasources/CDITravel" pool-name="CDITravelPool" enabled="true" use-java-context="true">
	<connection-url>jdbc:mysql://localhost:3306/cditravel</connection-url>
	<driver>mysql</driver>
	<security>
		<user-name>marvin</user-name>
		<password>marvin</password>
	</security>
</datasource>
 
This project uses [Maven](https://maven.apache.org/) as a library dependence manager. So, the libraries used in this project are described in `pom.xml` file.
 
# Testing
The application is available at address [http://localhost:8080/CDITravel(http://localhost:8080/CDITravel).
 
# Team
Fabio da Costa Pinto
Sirhan Bortolini
