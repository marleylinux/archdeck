# archdeck
Tutorial / Tips for the steamdeck running regular archlinux

Install arch as normal
-------------------------------------------------------------------------------------------------------------
go through this includes mostly everything plus binds efor buttons such as the power button
https://wiki.archlinux.org/title/Steam_Deck

Use ryzenadj / lact or both for gpu / apu clocks/limits
Use cpupower and edit /etc/defualt/cpupower (as the cpupower using -d and -u sets the clocks really low for me but the service works so edit the file to your needs)

#Audio fix
I read about the audio of the steamdeck being a lot quieter as compared to when on steamos and even 150% arch volume causes crazy crackling. A
On arch if you install alsa-utils and then do alsamixer then you can fix this.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
using alsa-mixer you need to find the two left pcn's and the two right pcn's (I wouldn't touch anything else) I personally turned them up to max, this causes a really loud and not crackling steamdeck (I'd say normal but it sounds very slightly off, maybe valve do some better or more cutom mixing)  but overall a a night and day difference

#Extra
steamdeck display in hyprland is eDP-1 

an example bind to make hyprland suspend would be: bind = , XF86PowerOff, exec, systemctl suspend 
volume buttons are XF86AudioRaiseVolume and XF86LowerVolume
