### Install dependencies

The simulator needs Ubunthu 16.04

packages to install (apt-get)

(Note you have to add sources as descirbed in the ros wiki)

```
$ sudo apt-get install ros-kinetic-desktop-full
$ sudo apt-get install ros-kinetic-joy
$ sudo apt-get install ros-kinetic-fake-localization
```

### Install gazebo-8

Then gazebo-8 is required **AND NOT** gazebo-7 which comes
with ros-kinetc. Installing gazebo-8 will remove gazebo-7.

[**instruction:**](http://gazebosim.org/tutorials?tut=install_ubuntu)

```
$ sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu-stable `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-stable.list'
$ wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -
$ sudo apt-get update
$ sudo apt-get install ros-kinetic-gazebo8-ros-pkgs
$ sudo apt-get install ros-kinetic-gazebo8-ros-control
```

Check you installation of gazebo:

```
$ gazebo
```

It should say version 8.1 or a newer version.
