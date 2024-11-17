# Fedora_posinstall
Some Post Installation Automation Using Ansible. in progress of adding more stuff

Including:
- install tmux, copy tmux configurations to ~/.tmux.conf file, Please change the contents inside tmux/tmux.conf to fit it as you like.
- install geany, copy geany theme to geany config from geany/ , you can change it and download themes from geany official site.
- I like dark mode, in Fedora 41, using gnome, when you change the geany theme still some parts are white, so darkmode role will take care of that. this will be applied system wide so bluefish, bless,... mostly will appear in dark mode.
- Nekoray VPN application install. the reason I didn't used the git module is that, cloning will move to nekoray 4 which is beta and on my system it's not working currectly, so I decided to use the get_url and download the release one.
