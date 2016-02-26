##xmlmc-rb-samples

These are a set of sample scripts that implement SupportWorks XMLMC interface using Ruby. These scripts can be use to
Populate demo call data into SupportWorks, Simulate active use in a demo system, test the XMLMC API whatever else

Naturally since these are ruby scripts, ruby is required. Ruby comes standard on Linux/Unix but can be installed for windows from

http://rubyinstaller.org/downloads/

For these scripts to run you need to install the xmlmc-rb gem, included in this package. To do that, download this repository
Unzip and run the command gem install [path to gemfile]\xmlmc-rb-2.0.0.gem

**Please be aware that this gem is still in active development and early test phases. These scripts have been tested, but they should
__not__ be used unless you are confident you know what you are doing**

To run the scripts use the command:

ruby [path to script]\[script to run].rb

To simulate active use in the system use supportworks scheduler.

###Configuration

Each script has a section that looks like this

```ruby
##
# Change these details to match your environment!! The first option needs to be the hostname or ip address
# of your server. The second option 'analyst_logon' needs to be set to the username and password of an administrator
# Failure to adjust these settings correctly could prevent the script from working or worse, make unwanted changes to
# your production environment
##

endpoint = '10.3.200.20'
username = 'admin'
password = ''
priority = 'P3 - Gold 4 Hr Resp. 8 Hr Fix - 9am - 5.30pm Mon- Fri'
```

These settings need to be changed to match your environment for the scripts to work.