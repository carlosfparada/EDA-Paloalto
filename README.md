# EDA-Paloalto Demo
#
## PANOS SETUP
# Login to the device with the default username and password (admin/admin). 
# When asked, set new password as follows:
#   admin/Cisco123
# Enter configuration mode
#   admin@fw> configure
# Change the system setting to static (DHCP is enabled by default) 
#   admin@fw# set deviceconfig system type static
# Use the following command to set the IP address of the management interface:
#   admin@fw# set deviceconfig system ip-address 172.16.2.211 netmask 255.255.248.0 default-gateway 172.16.1.1 dns-setting servers primary 8.8.8.8
# Commit the changes using the command
#   admin@fw# commit
# Exit configuration mode by using the command exit and then confirm the configurations by running the command show interface management within configuration mode
# admin@fw> show interface management
# admin@fw> show system info
#
# DEMO
# RUN panos_setup
# START EDA Rule activation
# add/delete policy rules: they will remain unchanged