# Infoblox Demo

## Configure the basic settings for a new instance of Infoblox NIOS 

1. Power up a new, unconfigured instance of Infoblox NIOS. Once it has finished booting, login at the prompt with the username `admin` and the password `infoblox`

```console
Disconnect NOW if you have not been expressly authorized to use this system.
login: admin
Local password:

               Infoblox NIOS Release 9.0.3-50212-ee11d5834df9 (64bit)
     Copyright (c) 1999-2023 Infoblox Inc. All Rights Reserved.

                   type 'help' for more information


Infoblox >
```
2. Configure any necessary license information with the `set license` or `set temp_license` command. For this example using a virtual NIOS appliance, temporary 60-day licenses activated. 
3. Option 2 below is selected first (DNSOne with Grid (DNS, DHCP, Grid)).

```console
Infoblox > set temp_license

  1. DNSone (DNS, DHCP)
  2. DNSone with Grid (DNS, DHCP, Grid)
  3. Network Services for Voice (DHCP, Grid)
  4. Add NIOS License
  5. Add DNS Server license
  6. Add DHCP Server license
  ...<truncated>

Select license (1-18) or q to quit: 2

This action will generate a temporary 60-day DNSone with Grid license.
Are you sure you want to do this? (y or n): y
DNS temporary license installed.
DHCP temporary license installed.
Grid temporary license installed.

Temporary license is installed.

The UI needs to be restarted in order to reflect license changes.
Restart UI now, this will log out all UI users? (y or n):y

Are you sure you want to do this? (y or n): y
UI restarted.
```
4. Option 4 below is selected next (Add NIOS License) followed by option 5 (IB-V825)

```console
Infoblox > set temp_license

  1. DNSone (DNS, DHCP)
  2. DNSone with Grid (DNS, DHCP, Grid)
  3. Network Services for Voice (DHCP, Grid)
  4. Add NIOS License
  5. Add DNS Server license
  6. Add DHCP Server license
  ... <truncated>

Select license (1-18) or q to quit: 4

  1. CP-V805
  2. IB-V805
  3. ND-V805
  4. IB-V815
  5. IB-V825
  6. ND-V906
  ... <truncated>
Enter a number corresponding to a NIOS model (1 - 29) or q to quit: 5

This action will generate a temporary 60-day NIOS (Model IB-V825) license.

WARN: The product needs to be restarted in order to reflect this license change.

Are you sure you want to do this? (y or n): y
NIOS temporary license installed.

Temporary license is installed.

System will RESTART shortly. Wait for RESTART completion and perform the required additional configuration
```