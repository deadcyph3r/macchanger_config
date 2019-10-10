# macchanger_config
Setting to change mac address on every boot 
# Macchanger
ifconfig eth0 gives your macaddress of your device
awk is used to format the results.
tool called macchanger is availabe in kali
for help type macchanger --help
Explore the tool's different availabe options.
To get a custom mac address follow this command.
macchanger --mac=XX:XX:XX:XX:XX:XX
To change mac address on everyboot:
crontab --help
crontab -e
 read entire file 
press i to insert
and then add the following command at the end of the file
 @reboot macchanger -r eth0
then press esc key
then type following command to write and quit
:wq
and if above command doesn't works type following command
:wq! 
to force write.
Congrats you have set up a macchanger to change your mac on every boot.
