# Basim

Click on Download Apache Maven you will be redirected to -->> https://maven.apache.org/download.cgi 
--------------
Step 1: Go to ec2 instance -->> cd /usr/local/share/
step 2: create directory (mkdir maven) execute a command below:
sudo mkdir maven
cd maven

step 3: sudo wget https://dlcdn.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.tar.gz

step 4: sudo tar -xvf apache-maven-3.9.6-bin.tar.gz

step 5: sudo vi /etc/profile  

JAVA_HOME="/usr/lib/jvm/java-1.8.0-openjdk"
M2_HOME="/usr/local/share/maven/apache-maven-3.9.6"
PATH=$PATH:"/usr/lib/jvm/java-1.8.0-openjdk":"/usr/local/share/maven/apache-maven-3.9.6/bin"

step 6: sudo update-alternatives --install "/usr/bin/mvn" "mvn" "/usr/local/share/maven/apache-maven-3.9.6/bin/mvn" 0 


step 7: sudo update-alternatives --set mvn /usr/local/share/maven/maven/apache-maven-3.9.6/bin/mvn 

step 8: mvn --version
