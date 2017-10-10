Vagrant.configure("2") do |config|
	 config.vm.define "box1" do |box1|

         box1.vm.box="ubuntu/trusty64"

         box1.vm.network :forwarded_port, guest: 22, host: 10122, id: "ssh"

 end


  config.vm.define "box2" do |box2|

         box2.vm.box="scotch/box"

         box2.vm.network :forwarded_port, guest: 22, host: 10222, id: "ssh"
 end
	
	#!/bin/bash
	echo "Please enter username:"
	read username
	echo "Please enter the new password:"
	read -s password1
	echo ""Please repeat the new password:""
	read -s password2
	# Check if both passwords match
	if [ $password1 != $password2 ]; then
	echo "Passwords do not match"
	exit    
	fi
	# Check if user exists
	id $username &> /dev/null
	if [ $? -eq 0 ]; then
	echo "$username exists... changing password."
	else
	echo "$username does not exist - Password could not be updated for $username";:          
	exit 
	fif
	# Change the password
	echo -e "$password1\n$password1" | passwd $username
end




#This is another edit! Mwahahaha!!!
#This is Svetlana's change!
