# Remote Maven Repository com JDBC Drivers

As últimas versões novas dos JDBC drivers da Oracle e do Firebird baixadas dos web sites dos donos no dia 01/07/2016, e transformados para formato Maven neste novo Remote Maven Repository. 
  
Estas versões não se encontram no Central Maven 2 Repository.
 
O transformador se encontra no outro projeto https://github.com/EricJoosse/Transformador-de-JDBC-drivers-para-Maven-artefacts.
 
Estes Maven artifacts podem ser referenciados em arquivos pom.xml da seguinte forma : 
```
  <repositories>
    <repository>
        <id>Remote-Maven-Repository-com-JDBC-Drivers</id>
        <url>https://raw.github.com/EricJoosse/Remote-Maven-Repository-com-JDBC-Drivers/mvn-repo/</url>
        <snapshots>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
        </snapshots>
    </repository>
  </repositories>

  <dependencies>
    <dependency>
    	<groupId>oracle.jdbc</groupId>
    	<artifactId>jdbc-oracle</artifactId>
    	<version>10.2.0.5.0</version>
    </dependency>
    <dependency>
    	<groupId>org.firebirdsql.jdbc</groupId>
    	<artifactId>jaybird-full</artifactId>
    	<version>2.2.10</version>
    </dependency>
  </dependencies>
```
