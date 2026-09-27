# First Boot

## After installation

1. Log in with your password (your username is auto-selected)
2. When logged in, connect to the internet for updates.
3. Open the terminal (if you can't find it, you can open the Applications Menu and search for 'Konsole'.)
4. Enter this command exactly as seen here:
```bash
sudo pacman-key --init
sudo pacman -Syu
```
Wait for it to finish up. When asked for a confirmation, type 'y' and press Enter (or just press Enter like that, pacman already assumes your answer is yes). If the updatess time out because of network, run 'sudo pacman -Syu' again.
5. When done, you're basically done setting up! 

<h4>Pointers on how to use pacman are in the documentation page "Updating".</h4>

