# Intel RAPL setting tool
Intel RAPL setting tool is a simple python script to configure Intel RAPL throught machine specific registries (MSR). It works for Intel processors on the Linux operating system.

Dependencies
============

It requires three dependencies to work:
- Python 2.7
- MSR module
- terminaltables module for python 

Install
----------

1) Enter in the main directory::

   >$ cd rapl_setting_tool
 
2) Make sure that the msr driver is loaded::

   $> sudo modprobe msr

3) Install terminaltables module for python

    $> sudo pip install terminaltables

4) Run the script with root permissions

    $> sudo ./rapl-set
