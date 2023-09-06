# jenkins
# Installing jenkins
->Using Dockerhub
   Download Jenkins and run image in a container
->Using Kubernetes(Open source sys for automating deployment scaling and management of containers)
   Download and install minikube
   Create minikube cluster
   Create a namespace
   Install jankins with Helm V3
   Create a persistent volume
   Create a service account
   Deploy jenkins
->Linux INSTALLERS(256mibs ram 1 gig harddrive , 4 gigs of ram 50gigs harddrive space)
  Debian/ubuntu
  Fedora
  RedHat/CentOS
->macOS
  2 diff builds
    Jenkins LTS
    Jenkins Weekly
->Using WAR Files
   Used with any supported Java Version
->Windows Installer
   Download from jenkinsio
->Other Os
   FreeBsd
   OpenIndiana Hipster
   Solaris,OmniOs,SmartOs etc
->Offline Installation
   Use WarFile


# Apache Tomcat Installation
  ->Required to deploy Jenkins WARFile
    Install java
    install apache tomcat
    Download and Deploy WarFile
    Install recommended Plugins

# Initial Settings
  ->jenkins settings
  ->Http settings



# Installing Jenkins In MacOS
  ->Install homebrew
    To check whether Installed
    * brew version
    * brew info
    * brew list
  * brew install nameofjenkins(jenkins-lts)
  * brew list
  * brew services list
  * brew services start nameofservice(jenkins-lts)
  -> Open browser ->localhost:8080
                  ->change directory to which we can see on localhost to find out password
                  ->Open file copy and paste password in browser
  ->Install suggested Plugins
  ->Create username and password
  ->start using jenkins

# Understanding Jobs
  ->Sequence of Configurations for running a particular task
  ->Automated tasks
  ->Jobs are blueprint for Builds
# Builds
  ->Single execution of tasks
  ->Every run is a build

  # Job to mean automation task and Build to mean single execution of the automation task at the current state of system and possibly some variables as input


  

    
  
 
