CentOS KVM Image Tools - README
===============================

+ Name: CentOS KVM Image Tools

+ Version: 1.0.000

+ Release date: 2013-04-23

+ Author: Nicola Asuni, Paul Maunders, Mark Sutton, Damion Parry

+ Copyright (2012-2013):

> > Fubra Limited
> > Manor Coach House
> > Church Hill
> > Aldershot
> > Hampshire
> > GU12 4RQ
> > <http://www.fubra.com>
> > <support@fubra.com>


SOFTWARE LICENSE:
-----------------

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.


DESCRIPTION:
------------

This project contains some simple tools, instructions and Kickstart configuration files to assist with creating CentOS KVM virtual machines.

## Installation

The following guide assumes you have virtualization tools such as virt-install, libguestfs and virt-sparsify installed.

If you don't, then install them:

    yum groupinstall "Virtualization Tools"
    yum install virt-manager libvirt libvirt-python python-virtinst virt-top libguestfs-tools
    reboot

## Build an image like so:

./centoscloud.sh CentOS-6.4-x86_64-20130712 CentOS-6.4-x86_64-cloud.cfg

