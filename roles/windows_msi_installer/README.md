Role Name
=========

This ansible role will help the windows admins to install MSI package.

Requirements
------------

Requirements for windows hosts: 
>  PowerShell 3.0
>  .NET 4.0
>  WinRM Configuration

To access windows host, please check https://ansible.com/blog/connecting-to-a-windows-host

Role Variables
--------------

Defaults variable created just for counters, to count installed, existing installation, failed status.

Roles variables are

MSI_File_Location:		# Specify Msi file location here
Inventory_group: 		# If windows team wants to install on specific group. 
MSIEXEC_arguments:		# arguments, if any. Most of the time you no need to set
Product_Code:			# mention product code of msi withing quotation and braces


Dependencies
------------

-Nil-

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: MSI_Windows_Installer }

License
-------

GPL 2.0

Author Information
------------------

Created by : Somasundaram  R. 
Please make necessary changes or mail me at tomsomu@gmail.com

[![CI](https://travis-ci.org/somusundaramr/MSI_Windows_Installer.svg?branch=master)](https://travis-ci.org/github/somusundaramr/MSI_Windows_Installer)
