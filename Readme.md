# Installing Logitech Media Server / Slimserver on Raspberry Pi

## Software

Logitech Media Server is developed on:

 *  https://github.com/Logitech/slimserver

Installable packages for a number of OS'ses are maintained by Logitech:

 * https://www.mysqueezebox.com/download

Unfortunately the debian version doesn't run on Raspberry Pi despite containing arm
perl XS stuff.

So downlaod a nightly build specifically built for ARM.

  $ wget -O logitechmediaserver_all.deb $(wget -q -O - "http://www.mysqueezebox.com/update/?version=7.9.0&revision=1&geturl=1&os=deb")

Install with dpkg

  \# dpkg -i logitechmediaserver_all.deb

## Hardware and OS

I have done the installation on a Raspberry Pi 3 with Raspbian.

 * Raspberry Pi model 3
 * Raspbian GNU/Linux 9 (updated on 6 oct 2018)


