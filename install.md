On linux :

. Add epel repo : wget https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
. Install epel-repo : yum install ./epel-release-latest-*.noarch.rpm
. or Redhat : rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
. sudo su - (login as root)
. yum update
. yum install ansible -y

. useradd ansadmin
. passwd ansadmin
. ansadmin ALL=(ALL) NOPASSWD: ALL
. /etc/ssh/sshd_config -> passwrdauthenticatio : yes
. service sshd restart

ssh key exchange :

. ssh-keygen
. ssh-copy-id 172.31.30.41

Jenkins Linux install :

. sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
. sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
. sudo yum install jenkins -y
. http://ec2-34-216-126-112.us-west-2.compute.amazonaws.com:8080








