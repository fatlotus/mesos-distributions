#### Apache Mesos Distribution

This project contains distributions of the 0.13.0 Mesos master and slave for Mac OS X and Debian / Ubuntu Linux.

##### Mac OS X

On a Mac OS X machine,

* install the provided `.mpkg` on two machines;
* on the master,
  * run `/usr/sbin/mesos-master --webui_dir=/usr/share/mesos/webui`; and
* on the slave,
  * run `/usr/sbin/mesos-slave --master=**0.0.0.0:5050`.

##### Debian / Ubuntu Linux

On an Ubuntu or Debian machine,

* run `sudo dpkg -i mesos_0.13.0_amd64.deb || (sudo apt-get install -f && sudo dpkg -i mesos_0.13.0_amd64.deb`;
* on the master,
  * run `/sbin/mesos-master --webui_dir=/share/mesos/webui`; and
* on the slave,
  * run `/sbin/mesos-slave --master=**0.0.0.0:5050`.

##### License

This code is covered under the Version 2.0 Apache License.