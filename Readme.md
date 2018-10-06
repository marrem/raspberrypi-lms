# Installing Logitech Media Server / Slimserver on Raspberry Pi

## Software

Logitech Media Server is developed on:

 *  https://github.com/Logitech/slimserver

Installable packages for a number of OS'ses are maintained by Logitech:

 * https://www.mysqueezebox.com/download

Unfortunately the debian version offered in the main download page  doesn't run on my Raspberry Pi 3

So download a nightly build:

  $ wget -O logitechmediaserver_all.deb $(wget -q -O - "http://www.mysqueezebox.com/update/?version=7.9.0&revision=1&geturl=1&os=deb")

See also: https://variax.wordpress.com/2017/02/24/install-lms-on-raspberry-pi/

Install with dpkg

  \# dpkg -i logitechmediaserver_all.deb

## Hardware and OS

I have done the installation on a Raspberry Pi 3 with Raspbian.

 * Raspberry Pi model 3
 * Raspbian GNU/Linux 9 (updated on 6 oct 2018)


## Plugins

Most just work after installing.

But the Shairtunes doesn't work 'out of the box'. It displays a 404 page not found
when trying to reach the settings. Strangely this was solved by installing:

libcrypt-openssl-rsa-perl

with the package manager...


