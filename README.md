# Jenkins
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

  ...Job to mean automation task and Build to mean single execution of the automation task at the current state of system and possibly some variables as input

# Create a Build in jenkins
 ->Search password in initialadminpassword
 ->Enter in jenkins(localhost)
 ->Change Password in jenkins
   Admin
   Configure
   change password
->Click newitem
->Enter item name
->In execute shell
   windows bash command
   echo "  "//all commands req to execute code
->Apply and save
->Build now

# Jenkins and Security
 ->Controller isolation : each build must be isolated from one another
 ->User Interface:(default)-->CSRF protection,Markup formatter,Rendered user content
 
# Securing Jenkins Environment
 ->Manage jenkins
 ...Making local computer as controller and send instructions so that other computers and run and create builds on them(Controller isolation)--(Inadvisable for long run)
 ->Manage nodes and clouds
 ->New node
 ->Permanent Agent
 ->Launch method --via ssh--127.0.0.1(optional)
 Access Controls
 ->Manage jenkins
 ->create user 
 ->right click and configure

# Jenkins Build Distribution
..Adding extra machines as needed
..Absorbing extra load dynamically
 ->Primary/Secondary Architecture
    ..primary deals with actual software computer/server where jenkins installed
    ..secondary doing all work for build distributions(Workers)-->Take instructions from primary node
 ->Secondary Agent
   Doesnt contains any jenkins software
   Get info from primary node
->Why needed?
 ..less latency,fault tolerance,availability,Scalability,Efficiency,durability

 # Distributed Jenkin Builds
 ..Uses agent
->Connecting to agent
     ->Manage jenkins
    ...Making local computer as controller and send instructions so that other computers and run and create builds on them(Controller isolation)--(Inadvisable for long run)
    ->Manage nodes and clouds
    ->New node
    ->Permanent Agent
    ->Launch Method via ssh
      ->paste ec2 instance from aws
      ->add credentials
        username with private key
        in key copy and paste ssh key
      ->credentials ..elias
# Jenkins Fingerprints and Artifacts 
  ->File version---Tracking files is done using fingerprinting
  ->Dependency version
  How to do
  ->Record fingerprits jar files
  ->Record everything
  How fingerprints work
  ->MD5 checksum
  ->Jenkins maintained database

  How to Record Fingerprints
  ->Click 'Configure'
  ->Scroll to post-build actions
  ->Select record fingerprint of files

  Test and Artifacts
  ->Jenkins help by recording aggregate test results

  Recording and Tests and Artifacts
  ->Using Junit or Plugins
  
# Managing Jenkins Fingerprints and Artifacts 
  ->Create build
  ->In Add post-build actions
    ..Select Record fingerprints
    ..*.py(All python fingerprints will be fingerprinted)
    
  
        
 
    
 
  


  

    
  
 
