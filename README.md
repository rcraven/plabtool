# plabtool

<img src="http://codeen.cs.princeton.edu/PlanetLab_logo1.jpg" alt="Note: plabtool is my personal script and not endorsed by PlanetLab" title="Note: plabtool is my personal script and not endorsed by PlanetLab" align="right">

plabtool is a Python script that makes it easy for you to administer your PlanetLab slice from the command line.  plabtool is essentially a frontend interface to the [PlanetLab Central API].

plabtool supports the following actions:

- **Get Info** about your slice or a specific node
- **Renew** your slice
- **List** the nodes assigned to your slice in a [PSSH]-friendly format
- **Add** your slice to a single node or list of nodes in a file
- **Delete** your slice from a node
- **Swap** out a node for another one at the same site (shows you a list and lets you choose)
- **Purge** all nodes from your slice
- **List sites** where your slice has a presence
- **Add site-unique nodes** to your slice.  Fill your slice with as many site-unique node as possible while optionally avoiding any nodes listed in your blacklist.  This feature was created to automate the process of avoiding duplicate nodes at the same site, ensuring maximum geographic diversity of nodes in the slice.

## Setup
plabtool is just a simple Python script, so no installation is required.  Just make sure you have Python installed, download the script, configure it, and run it.

To configure the script:

1. Edit the top section of the script marked *PROGRAM SETTINGS*.  Be sure to include your:
  * Slice name
  * PlanetLab username
  * **Optionally:** PlanetLab password in a file (*chmod 400* the password file)
2. That's it, have fun!

## Copyright and License
This software is &copy; 2014 Ryan Craven and released under the [MIT license]

[PlanetLab Central API]: https://www.planet-lab.org/doc/plc_api
[PSSH]: https://code.google.com/p/parallel-ssh/
[MIT license]: http://choosealicense.com/licenses/mit/
