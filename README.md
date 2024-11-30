# Fedora_posinstall
Some Post Installation Automation Using Ansible. in progress of adding more stuff

Before using this please do the following:

<code>
sudo dnf -y update
sudo dnf install -y ansible
</code>
<br>
Including:
- install and configure the Fedora repos, including rpm-fusion-free, rpm-fusion-nonefree and rpmsphere repos. as this is aimed for Fedora 41 the activation of openh264 library is different with older versions of Fedora.
- install tmux, copy tmux configurations to ~/.tmux.conf file, Please change the contents inside tmux/tmux.conf to fit it as you like.
- install geany, copy geany theme to geany config from geany/ , you can change it and download themes from geany official site.
- I like dark mode, in Fedora 41, using gnome, when you change the geany theme still some parts are white, so darkmode role will take care of that. this will be applied system wide so bluefish, bless,... mostly will appear in dark mode.
- Nekoray VPN application install. the reason I didn't used the git module is that, cloning will move to nekoray 4 which is beta and on my system it's not working currectly, so I decided to use the get_url and download the release one.
