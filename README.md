7zip
anaconda2
anaconda3
cmder
docker
docker-cli
docker-compose
docker-desktop
docker-engine
dotnet3.5
dotnet4.5
drawio
eclipse
filezilla
git
golang
googlechrome
intellijidea-community
javadecompiler-gui
jmeter
kind
kubernetes-helm
lens
maven
mcr-r2019a
mobaxterm
msvisualcplusplus2012-redist
msvisualcplusplus2013-redist
netfx-4.8
nodejs
notepadplusplus
office365business
openjdk11
openjdk8
pip
postman
powerbi
putty
python
soapui
sql-server-management-studio
sublimetext2
sublimetext3
sublimetext4
vcredist2008
vcredist2010
vcredist2012
vcredist2015
vcredist2017
visualcplusplusexpress2008
visualstudio2017professional
visualstudio2019community
visualstudio2019professional
visualstudio2022professional
vscode
wildfly
winmerge
wsl
wsl2
xmind
zulu11
zulu7
zulu8



foreach($line in Get-Content .\name.txt) {
if($line -match $regex) {
choco install $line -s http://url/ -u "name" -p "password" -y
}}



 cat chocolatey.log | grep -iE "^Chocolatey installed|Installing the following packages:$" -A 1
