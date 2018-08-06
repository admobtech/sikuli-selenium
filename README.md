# sikuli-selenium
Maven-Sikuli-Selenium

<repositories>
        <repository>
      <!-- OSSRH: com.sikulix -->
           <name>com.sikulix</name>
           <id>com.sikulix</id>
           <url>https://oss.sonatype.org/content/groups/public</url>
           <layout>default</layout>
           <releases>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </releases>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>


  <dependencies>
   <dependency>
     <groupId>junit</groupId>
     <artifactId>junit</artifactId>
     <version>3.8.1</version>
     <scope>test</scope>
    </dependency>

   <dependency>
     <groupId>org.testng</groupId>
      <artifactId>testng</artifactId>
     <version>6.8</version>
   </dependency>

   <dependency> 
       <groupId>com.sikulix</groupId>
       <artifactId>sikulixapi</artifactId>
       <version>1.1.0-SNAPSHOT</version>          
    </dependency>
 </dependencies>

 <build>
   <plugins>
    <plugin>
        <groupId>org.testngorg.apache.maven.plugins</groupId>
        <artifactId>maven-compiler-plugin</artifactId>
        <version>3.3</version>
        <configuration>
            <source>1.5</source>
            <target>1.5</target>
        </configuration>    
    </plugin>

    <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-surefire-plugin</artifactId>
        <version>2.4.2</version>
        <configuration>
            <siuteXmlFiles>
                <suiteXmlFile>testng-customsuite.xml</suiteXmlFile>
            </siuteXmlFiles>
        </configuration>    
    </plugin>
</plugins>
