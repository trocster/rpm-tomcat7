rpm-tomcat7
===========

An RPM spec file to install Tomcat 7.0.78

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`wget https://raw.github.com/trocster/rpm-tomcat7/master/tomcat7.spec -O ~/rpmbuild/SPECS/tomcat7.spec --no-check-certificate`

`wget https://raw.github.com/trocster/rpm-tomcat7/master/tomcat7.init -O ~/rpmbuild/SOURCES/tomcat7.init --no-check-certificate`

`wget https://raw.github.com/trocster/rpm-tomcat7/master/tomcat7.sysconfig -O ~/rpmbuild/SOURCES/tomcat7.sysconfig --no-check-certificate`

`wget https://raw.github.com/trocster/rpm-tomcat7/master/tomcat7.logrotate -O ~/rpmbuild/SOURCES/tomcat7.logrotate --no-check-certificate`

`wget http://mirror.ox.ac.uk/sites/rsync.apache.org/tomcat/tomcat-7/v7.0.77/bin/apache-tomcat-7.0.77.tar.gz -O ~/rpmbuild/SOURCES/apache-tomcat-7.0.77.tar.gz`

`rpmbuild -bb ~/rpmbuild/SPECS/tomcat7.spec`
