# hello
practical 1

# Install Virtual box/VMware Workstation with different flavours of linux or windows OS on top of windows.

https://www.virtualbox.org/ 

1. download by clicking on windows host
2. install
3. http://ubuntu.com/download/desktop
4. ubuntu-24 iso file
5. click new in virtual box give name
6. after next go to setting of that ubuntu and make shared clipboard and drag an drop bi directional

![image.png](attachment:780c8641-c9b0-47d5-84a1-3efe6e075689:image.png)

1. go to storage do this and add iso file there in choose virtual optical disk
2. after start it and install 

# 2.  Installation and configure Google App Engine. Create hello world app and other simple web applications using python/java.

download installer in it

https://appengine.google.com/

https://www.npackd.org/p/com.google.AppEnginePythonSDK/1.9.62

donload google app engine go to edit click preferences

give pyhton path python .exe 

give path of app engine go in programfile in google app engine and give path

create a app folder

now in file addnew application give directory to new file

check python version 

download python 2.7

pip install flask or check 

open vs code

create a directort mkdir my-flask-app

create [main.py](http://main.py) in it

```jsx
from flask import Flask
```

```jsx
app = Flask(__**name**__)
```

```jsx
@app.route(’/’)
def hello():
	return "hello, america ya"

if __name__ == "main":
	app.run(host = "127.0.0.1", port = 8080, debug=True)
```

now create app.yaml fime

```jsx
runtime : python39
entrypoint: python main.py

handlers: 
- url: /.*
	script: auto
```

change directory

python main.py

# 5. Implement network virtualization using VirtualBox

install 2 like ubuntu and kali

file> host network manager> create

dhcp server> check enable server

change 54 to 100>  PPLY

![image.png](attachment:0cceb1d0-4d73-4867-87b7-2562e2849f20:image.png)

got to adapter> configure adapter automatically>apply

![image.png](attachment:6268f907-70d2-44c7-8aee-88b8a2f3ac66:image.png)

select v machine

uncheck adapter 1

go to network setting> go to adapter 2> eanble the adapter

do this setting on both

![image.png](attachment:b43868c9-1e0f-4bfe-8380-4ee490e9ce00:image.png)

```jsx
ip addr show
```

show we can se host has obtained ipaddress from subnet range

```jsx
ping 192.168.100.4 -c 5 
```

to check if they are connected do on another v machine too

# 7. Installation and Configuration of virtualization using KVM.

[How to Install KVM on Ubuntu | phoenixNAP KB](https://phoenixnap.com/kb/ubuntu-install-kvm)

update ubuntu 

sudo apt update

sudo apt upgrade

egrep -c’(vmx|svm)’ /proc/cpuinfo

kvm-ok ,  if not then

sudo apt install cpu-checker

kvm-ok 

sudo apt install qemu-kvm virt-manager libvirt-daemon-system virtinist libvirt-clients bridge-utils

sudo systemctl enable - -now libvirtd

sudo systemctl start libvirtd

sudo systemctl status libvirtd

sudo usermod -aG kvm $USER

sudo usermod -aG libvirt $USER

log out and log in

virtual machine amanger

kubernetes

[How to Install Kubernetes(K8s) and Docker on Ubuntu 20.04 - LetsCloud Community](https://www.letscloud.io/community/how-to-install-kubernetesk8s-and-docker-on-ubuntu-2004)

# Find a procedure to transfer the files from one virtual machine to another virtual machine.

install winscp 

open oracle ivrtual box open ubuntu 

sudo apt install openssh-server

ifconfig
