# Xresources
To reload ...
```xrdb ~/.Xresources```
# Inputs ...
To list devices:
```
sudo xinput list.
```
To list device properties.
```
sudo xinput list-props <device-name>
```
To set a propertie.
```
sudo xinput --set-prop <device-name> <device-propertie>
```
# Assign an application to a workspace
First we need no detect which class the application's window belongs to.<br>
To to this run the command `xprop` and click on the desired window. Copy the second value of `WM_CLASS`.<br>
Addo  to `i3` config file:
```
assign [class=<class-name>] <workspace>
```
# Fonts!
Download Font-Awesome !
```
wget https://github.com/FortAwesome/Font-Awesome/releases/download/5.7.2/fontawesome-free-5.7.2-desktop.zip
```
Copy the `.ttf` or the `.otfs` to `~/.fonts`.
```
wget https://github.com/supermarin/YosemiteSanFranciscoFont/archive/master.zip
```
## Audio
```
git clone https://github.com/haikarainen/light ~/.light
cd ~/.ligth
./autogen.sh
./configure && make
sudo make install
```
# i3bars
## Volume
Install pavucontrol (pulse audio control). Run the volume script passing 5 and pulse as parameters.


