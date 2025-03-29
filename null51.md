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


eyJpY2VfY2FuZGlkYXRlcyI6W10sIm9mZmVyIjoie1wic2RwXCI6XCJ2PTBcXHJcXG5vPS0gNTM4Mjg1MzE0ODE0MDM4NTg5MCAyIElOIElQNCAxMjcuMC4wLjFcXHJcXG5zPS1cXHJcXG50PTAgMFxcclxcbmE9Z3JvdXA6QlVORExFIDBcXHJcXG5hPWV4dG1hcC1hbGxvdy1taXhlZFxcclxcbmE9bXNpZC1zZW1hbnRpYzogV01TXFxyXFxubT1hcHBsaWNhdGlvbiA5IFVEUC9EVExTL1NDVFAgd2VicnRjLWRhdGFjaGFubmVsXFxyXFxuYz1JTiBJUDQgMC4wLjAuMFxcclxcbmE9aWNlLXVmcmFnOkx2bFNcXHJcXG5hPWljZS1wd2Q6RWpDOURhVmpMeWg1Y0xvVFUxZzhCK2lXXFxyXFxuYT1pY2Utb3B0aW9uczp0cmlja2xlXFxyXFxuYT1maW5nZXJwcmludDpzaGEtMjU2IDI1OjIyOkMzOkQ4OjU5OjEzOjI0OjdGOjVBOjMzOkI0OkUwOkFGOjEyOjlEOkFEOjAxOjBEOkY3OjU4OjJGOjRGOjVFOkI5OjI3OjBFOjRBOkFCOkVBOjhGOkE1OkY1XFxyXFxuYT1zZXR1cDphY3RwYXNzXFxyXFxuYT1taWQ6MFxcclxcbmE9c2N0cC1wb3J0OjUwMDBcXHJcXG5hPW1heC1tZXNzYWdlLXNpemU6MjYyMTQ0XFxyXFxuXCIsXCJ0eXBlXCI6XCJvZmZlclwifSJ9
