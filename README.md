# cicd
**
Sonarqube installation 
Sonar Installation
Method -1
docker run --name sonarqube-custom -p 9000:9000 sonarqube:community**
----------------------------------------------------------------

Method -2

wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-25.1.0.102122
unzip *
chmod -R 755 /home/sonarqube/sonarqube-25.1.0.102122
chown -R sonarqube:sonarqube /home/sonarqube/sonarqube-25.1.0.102122
cd sonarqube-25.1.0.102122/bin/linux-x86-64/
./sonar.sh start

# cd /home/sonarqube/sonarqube-25.1.0.102122/bin/linux-x86-64
# bash ./sonar.sh start
-------------------------------------------------------------


To check the Sonar port is running or not
netstat -an | grep 9000 | grep LISTEN
