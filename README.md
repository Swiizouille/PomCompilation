# PomCompilation
POM.xml compilation bungeecord



<-------------------------------BungeeCord------------------------------->

<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>net.name</groupId>
    <artifactId>PluginName</artifactId>
    <version>1.0-SNAPSHOT</version>

    <repositories>
        <repository>
            <id>bungeecord-repo</id>
            <url>https://oss.sonatype.org/content/repositories/snapshots</url>
        </repository>
    </repositories>

    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.8.1</version>
                <configuration>
                    <source>1.8</source>
                    <target>1.8</target>
                </configuration>
            </plugin>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-shade-plugin</artifactId>
                <version>3.2.4</version>
                <executions>
                    <execution>
                        <phase>package</phase>
                        <goals>
                            <goal>shade</goal>
                        </goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>



    <dependencies>
        <dependency>
            <groupId>net.md-5</groupId>
            <artifactId>bungeecord-api</artifactId>
            <version>1.16-R0.5-SNAPSHOT</version>
            <type>jar</type>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>net.md-5</groupId>
            <artifactId>bungeecord-api</artifactId>
            <version>1.16-R0.4</version>
            <scope>provided</scope>
        </dependency>
    </dependencies>

</project>



<-------------------------------Spigot------------------------------->

<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>net.name</groupId>
    <artifactId>PluginName</artifactId>
    <version>1.0-SNAPSHOT</version>

    <repositories>
        <repository>
            <id>bungeecord-repo</id>
            <url>https://oss.sonatype.org/content/repositories/snapshots</url>
        </repository>
    </repositories>

    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.8.1</version>
                <configuration>
                    <source>1.8</source>
                    <target>1.8</target>
                </configuration>
            </plugin>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-shade-plugin</artifactId>
                <version>3.2.4</version>
                <executions>
                    <execution>
                        <phase>package</phase>
                        <goals>
                            <goal>shade</goal>
                        </goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>


    <repositories>
    <!-- This adds the Spigot Maven repository to the build -->
    <repository>
        <id>spigot-repo</id>
        <url>https://hub.spigotmc.org/nexus/content/repositories/snapshots/</url>
    </repository>
</repositories>

<dependencies>
    <!--This adds the Spigot API artifact to the build -->
    <dependency>
           <groupId>org.spigotmc</groupId>
           <artifactId>spigot-api</artifactId>
           <version>1.16.5-R0.1-SNAPSHOT</version>
           <scope>provided</scope>
    </dependency>

</project>


