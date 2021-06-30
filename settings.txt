<?xml version="1.0" encoding="UTF-8"?>

<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
          xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 http://maven.apache.org/xsd/settings-1.0.0.xsd">
  
  <servers>
    <server>
      <id>central</id>
      <username>admin</username>
      <password>password</password>
    </server>
    <server>
      <id>snapshots</id>
      <username>admin</username>
      <password>password</password>
    </server>
  </servers>

  <profiles>
    <profile>
      <repositories>
        <repository>
          <snapshots>
            <enabled>false</enabled>
          </snapshots>
          <id>central</id>
          <name>maven-repo</name>
          <url>http://3.21.186.209:8081/artifactory/maven-repo</url>
        </repository>
        <repository>
          <snapshots>
            <enabled>false</enabled>
          </snapshots>
          <id>snapshots</id>
          <name>maven-repo</name>
          <url>http://3.21.186.209:8081/artifactory/maven-repo</url>
        </repository>
      </repositories>
      <pluginRepositories>
        <pluginRepository>
          <snapshots>
            <enabled>false</enabled>
          </snapshots>
          <id>central</id>
          <name>maven-repo</name>
          <url>http://3.21.186.209:8081/artifactory/maven-repo</url>
        </pluginRepository>
        <pluginRepository>
          <snapshots>
            <enabled>false</enabled>
          </snapshots>
          <id>snapshots</id>
          <name>maven-repo</name>
          <url>http://3.21.186.209:8081/artifactory/maven-repo</url>
        </pluginRepository>
      </pluginRepositories>
      <id>artifactory</id>
    </profile>
  </profiles>
  <activeprofiles>
    <activeprofile>artifactory</activeprofile>
  </activeprofiles>
</settings>