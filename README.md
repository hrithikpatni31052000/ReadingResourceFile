Step 1 :
Add this above lines of code in your pom.xml
<plugins>
           <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-jar-plugin</artifactId>
                <version>3.2.0</version>
               <configuration>
                    <archive>
                        <manifest>
                            <addClasspath>true</addClasspath>-->
                            <!--<classpathPrefix>lib/</classpathPrefix>-->
                          <mainClass>com.springboot.fullstack.SpringBootFullStackApplication</mainClass>
                        </manifest>
                    </archive>
                </configuration>
            </plugin>

            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
                <version>2.6.0</version>
            </plugin>
</plugins>

Step 2:
command to create a jar : mvn package

Step 3:
Open cmd in target folder
run command : java -jar <Filename.jar> 
