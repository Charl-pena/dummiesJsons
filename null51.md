# Paso 1

Invoke-WebRequest -Uri https://downloads.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.zip -OutFile maven.zip

# Paso 2

Expand-Archive -Path maven.zip -DestinationPath "C:\Tools"

# Paso 3

$env:MAVEN_HOME = "C:\Tools\apache-maven-3.9.6"
[System.Environment]::SetEnvironmentVariable("MAVEN_HOME", $env:MAVEN_HOME, [System.EnvironmentVariableTarget]::Machine)

$env:Path += ";$env:MAVEN_HOME\bin"
[System.Environment]::SetEnvironmentVariable("Path", $env:Path, [System.EnvironmentVariableTarget]::Machine)

# Links

(https://github.com/codec-abc/Yew-WebRTC-Chat)

# Maven dependencias

<dependency>
    <groupId>org.apache.logging.log4j</groupId>
    <artifactId>log4j</artifactId>
    <version>2.24.3</version>
    <type>pom</type>
</dependency>
