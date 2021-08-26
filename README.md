# install xampp lampp in ubuntu

//Use This Link For Download xampp ubuntu

https://www.apachefriends.org/xampp-files/7.3.29/xampp-linux-x64-7.3.29-2-installer.run

// first if you disable password any time

sudo visudo

	%admin	ALL=(ALL) NOPASSWD:ALL
	
	%sudo	ALL=(ALL) NOPASSWD:ALL
	

//install xampp ubuntu
cd /home/youru-sername/Downloads
sudo chmod 755 xampp-linux-installer.run
sudo ./xampp-linux-installer.run

//create icon desktop
[Desktop Entry]
Encoding=UTF-8
Name=XAMPP Control Panel
Comment=Start and Stop XAMPP
Exec=sudo /opt/lampp/manager-linux-x64.run
Icon=/opt/lampp/htdocs/favicon.ico
Categories=Application
Type=Application
Terminal=false

//uninstall your current xampp 
sudo -i
cd /opt/lampp
sudo ./uninstall
