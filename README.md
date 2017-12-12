# Remote Maven Repository com JDBC Drivers

As últimas versões novas dos JDBC drivers da Oracle e do Firebird foram baixadas dos web sites dos donos no dia 01/07/2016, e o JCO driver do SAP do site do SAP no dia 12/12/2017. Os drivers foram transformados para formato Maven neste novo Remote Maven Repository. 
  
Estas versões não se encontram no Central Maven 2 Repository.
 
O transformador se encontra no outro projeto https://github.com/EricJoosse/Transformador-de-JDBC-drivers-para-Maven-artifacts.
 
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
    <dependency>
    	<groupId>com.sap</groupId>
    	<artifactId>jco-sap</artifactId>
    	<version>3.0.17</version>
    </dependency>
  </dependencies>
```
