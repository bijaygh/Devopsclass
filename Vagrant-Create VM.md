
Lotus@DESKTOP-JJN2VGS MINGW64 ~
$ cd bijay

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Importing base box 'ubuntu/focal64'...
==> default: Matching MAC address for NAT networking...
==> default: Checking if box 'ubuntu/focal64' version '20230506.0.0' is up to date...
==> default: Setting the name of the VM: bijay_default_1683563494951_11336
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
    default: Adapter 2: bridged
==> default: Forwarding ports...
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Running 'pre-boot' VM customizations...
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
    default: Warning: Connection reset. Retrying...
    default: Warning: Connection aborted. Retrying...
    default:
    default: Vagrant insecure key detected. Vagrant will automatically replace
    default: this with a newly generated keypair for better security.
    default:
    default: Inserting generated public key within guest...
    default: Removing insecure key from the guest if it's present...
    default: Key inserted! Disconnecting and reconnecting using new SSH key...
==> default: Machine booted and ready!
==> default: Checking for guest additions in VM...
    default: The guest additions on this VM do not match the installed version of
    default: VirtualBox! In most cases this is fine, but in rare cases it can
    default: prevent things such as shared folders from working properly. If you see
    default: shared folder errors, please make sure the guest additions within the
    default: virtual machine match the version of VirtualBox you have installed on
    default: your host and reload your VM.
    default:
    default: Guest Additions Version: 6.1.38
    default: VirtualBox Version: 7.0
==> default: Configuring and enabling network interfaces...
==> default: Mounting shared folders...
    default: /vagrant => C:/Users/Lotus/bijay

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ ls -al
total 24
drwxr-xr-x 1 Lotus 197609    0 May  8 22:15 ./
drwxr-xr-x 1 Lotus 197609    0 May  8 21:42 ../
drwxr-xr-x 1 Lotus 197609    0 May  8 22:15 .vagrant/
-rw-r--r-- 1 Lotus 197609 3087 May  8 22:15 Vagrantfile

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ ls -al .vagrant
total 4
drwxr-xr-x 1 Lotus 197609 0 May  8 22:15 ./
drwxr-xr-x 1 Lotus 197609 0 May  8 22:15 ../
drwxr-xr-x 1 Lotus 197609 0 May  8 22:15 machines/
drwxr-xr-x 1 Lotus 197609 0 May  8 22:15 rgloader/

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant ssh
Welcome to Ubuntu 20.04.6 LTS (GNU/Linux 5.4.0-148-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Mon May  8 16:39:51 UTC 2023

  System load:             0.0
  Usage of /:              3.7% of 38.70GB
  Memory usage:            21%
  Swap usage:              0%
  Processes:               115
  Users logged in:         0
  IPv4 address for enp0s3: 10.0.2.15
  IPv4 address for enp0s8: 192.168.1.80
  IPv6 address for enp0s8: 2400:1a00:b030:76e:a00:27ff:fe70:3a44


Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status

New release '22.04.2 LTS' available.
Run 'do-release-upgrade' to upgrade to it.


vagrant@ubuntu-focal:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 02:32:0f:32:b7:c0 brd ff:ff:ff:ff:ff:ff
    inet 10.0.2.15/24 brd 10.0.2.255 scope global dynamic enp0s3
       valid_lft 85959sec preferred_lft 85959sec
    inet6 fe80::32:fff:fe32:b7c0/64 scope link
       valid_lft forever preferred_lft forever
3: enp0s8: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 08:00:27:70:3a:44 brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.80/24 brd 192.168.1.255 scope global dynamic enp0s8
       valid_lft 85963sec preferred_lft 85963sec
    inet6 2400:1a00:b030:76e:a00:27ff:fe70:3a44/64 scope global dynamic mngtmpaddr noprefixroute
       valid_lft 1089sec preferred_lft 1089sec
    inet6 fe80::a00:27ff:fe70:3a44/64 scope link
       valid_lft forever preferred_lft forever
vagrant@ubuntu-focal:~$ ls /vagrant/
Vagrantfile
vagrant@ubuntu-focal:~$ cat vagrant/vagrantfile
cat: vagrant/vagrantfile: No such file or directory
vagrant@ubuntu-focal:~$ cat vagrant /vagrangfile/
cat: vagrant: No such file or directory
cat: /vagrangfile/: No such file or directory
vagrant@ubuntu-focal:~$ ls
vagrant@ubuntu-focal:~$ vagrant status

Command 'vagrant' not found, but can be installed with:

apt install vagrant
Please ask your administrator.

vagrant@ubuntu-focal:~$ cd vagrant
-bash: cd: vagrant: No such file or directory
vagrant@ubuntu-focal:~$ ls
vagrant@ubuntu-focal:~$ cd /vagrant/
vagrant@ubuntu-focal:/vagrant$ vagrant status

Command 'vagrant' not found, but can be installed with:

apt install vagrant
Please ask your administrator.

vagrant@ubuntu-focal:/vagrant$ vagrantfile hello.txt
vagrantfile: command not found
vagrant@ubuntu-focal:/vagrant$ ls
Vagrantfile
vagrant@ubuntu-focal:/vagrant$ touch hello.txt
vagrant@ubuntu-focal:/vagrant$ ls
Vagrantfile  hello.txt
vagrant@ubuntu-focal:/vagrant$ exit
logout

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ ls
Vagrantfile  hello.txt

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ pwd
/c/Users/Lotus/bijay

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant status
Current machine states:

default                   running (virtualbox)

The VM is running. To stop this VM, you can run `vagrant halt` to
shut it down forcefully, or you can run `vagrant suspend` to simply
suspend the virtual machine. In either case, to restart it again,
simply run `vagrant up`.

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant global-status
id       name    provider   state    directory
-------------------------------------------------------------------------
7ec285a  default virtualbox poweroff C:/Users/Lotus/Desktop/devops
333e2ec  default virtualbox running  C:/Users/Lotus/bijay

The above shows information about all known Vagrant environments
on this machine. This data is cached and may not be completely
up-to-date (use "vagrant global-status --prune" to prune invalid
entries). To interact with any of the machines, you can go to that
directory and run Vagrant, or you can use the ID directly with
Vagrant commands from any directory. For example:
"vagrant destroy 1a2b3c4d"

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant halt
==> default: Attempting graceful shutdown of VM...
vag
Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$ vagrant status
Current machine states:

default                   poweroff (virtualbox)

The VM is powered off. To restart the VM, simply run `vagrant up`

Lotus@DESKTOP-JJN2VGS MINGW64 ~/bijay
$
