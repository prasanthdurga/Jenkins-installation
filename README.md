# Jenkins-installation
step to install jenkins and java 


/usr/lib/jvm/java-8-openjdk-amd64

How to install java and set environment path for installation for jenkins

step 1 : launch ec2 instance with t2.micro either (linux or ubuntu)

step 2 : update the instances 
         yum update  --- linux
         sudo apt-get update.
step 3: install jave packages 
 
        sudo apt-get install -y openjdk-8-jre openjdk-8-jdk 

check java version : java -version && echo $JAVA_HOME

step 4 : go to this directory 

            cd /usr/lib/ls
            cd jvm/
            ls
and go to " cd java-8-openjdk-amd64/" 
next type ls bin/

next type "pwd"

we can see java home path copy that path. "/usr/lib/jvm/java-8-openjdk-amd64"

step 5 : type this command export JAVA_HOME= /usr/lib/jvm/java-8-openjdk-amd64

STEP 6: export PATH=$PATH:$JAVA_HOME/bin
        echo $PATH

STEP 7: TYPE sudo vi /etc/environment 

add this path "JAVA_HOME= /usr/lib/jvm/java-8-openjdk-amd64"

step 8:  sudo vi  ~/.bashrc

           add this one = "JAVA_HOME= /usr/lib/jvm/java-8-openjdk-amd64"
                           PATH=$PATH:$JAVA_HOME/bin
type this command source /etc/environment

step 9 : Follow the below URL FOR ADDING ADD AND INSTALATION OF JENKINS

https://wiki.jenkins.io/display/JENKINS//Installing%20Jenkins%20on%20Ubuntu

