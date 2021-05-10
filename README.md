# soft_dev
most software development code


# Packaging this code for android
#### follow the steps below from your terminal
$ pip install buildozer

$ buildozer init


check that your buildozer.spec file contains the following details

### (str) Title of your application
title = KvCalc

### (str) Package name
package.name = kvcalc

### (str) Package domain (needed for android/ios packaging)
package.domain = org.kvcalc


#### run the following
$ buildozer -v android debug



# Packaging this app for ios
$ brew install autoconf automake libtool pkg-config

$ brew link libtool

$ sudo easy_install pip

$ sudo pip install Cython==0.29.10

$ git clone git://github.com/kivy/kivy-ios

$ cd kivy-ios

$ ./toolchain.py build python3 kivy

#### if any errors, install openssl
$ cd /Applications/Python\ 3.7/

$ ./Install\ Certificates.command

#### use toolchain to create an entry point
./toolchain.py create <title> <app_directory>
