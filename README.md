Role Name
=========

Ansible role to install Jenkins on Debian/Redhat based OS. It checks the OS by using the ansible_facts['os_family'] fact and runs the tasks needed to install Java and Jenkins. It enables/starts the Jenkins server after installation.


Role Variables
--------------
Default variables are

default yum repo and key for redhat based OS

jenkins_yum_repo:
  url: "https://pkg.jenkins.io/redhat"
  
  key: "https://pkg.jenkins.io/redhat/jenkins.io-2023.key"
  
default java version for yum

java_yum_version: "java-17-openjdk"

default apt repo url for debian based OS

jenkins_apt_repo_url: "https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key"

default java version for apt

java_apt_version: "openjdk-17-jre"
