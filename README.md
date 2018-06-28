HackintoshOSX-MOTD
==================

Hackintosh OSX Message of the Day

## To Install

To install this script, there are two major steps that need to be completed:
  
  1. Copy `dynmotd` to `/etc` 
  
  2. Edit `/etc/profile` and at the end of `/etc/profile` add: `php -f /etc/dynmotd | bash`

When you open a new terminal, the new motd will be displayed.

**Note:** You can also move `dynmotd` to somewhere else on your path if you want.  Editing `/etc/profile` requires root privileges, but you can also add the line to `~/.bash_profile` replacing `/etc/dynmotd` with the path to `dynmotd`.  

## Next-Gen Message of the Day

The `dynmotd` script outputs a bash file that looks like the following when executed. It supports colors and variables, and parses the output of `system_profiler SPFirewallDataType SPPowerDataType SPNetworkDataType SPSoftwareDataType` to obtain system pertinent information and stored it into flattened variables.

      --  Hackintosh OS X --
         OS X 10.8.3 (12D78) 

    Network:
    Hostname: Splug’s MacBook Pro
    Addresses: 10.14.3.13
    Next-Hop: 10.14.3.1
    DNS Servers: 10.14.2.153, 10.14.3.154, 10.14.21.9, 10.13.21.9
    en0: 10.14.3.13
    Firewall: Limit incoming connections to specific services and applications

    System:
    Uptime: 29 days 8:39
    Processor:  Intel(R) Core(TM) i7-3740QM CPU @ 2.70GHz

    Battery:
    Charging: No
    Percentage: 87.03823807594%
    Splugs-MacBook-Pro:~ splug$
If you're on a desktop, you might see something like:

      --  Hackintosh OS X --
        macOS 10.13.5 (17F77)
    
    Network:
    Hostname: Mac Mini
    Addresses: 192.0.2.15
    Next-Hop: 192.0.2.5
    DNS Servers: 8.8.8.8, 8.8.4.4
    en1: 192.0.2.15
    Firewall: Allow all incoming connections

    System:
    Uptime: 12 days 56 minutes
    Processor:  Intel(R) Core(TM) i5-3210M CPU @ 2.50GHz
    
<!--  ![Example](http://www.highonphp.com/v3/wp-content/uploads/2013/06/Screen-Shot-2013-06-18-at-10.56.35-AM.png)-->
  

  
  
