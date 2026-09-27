# Updating

## Basic info on how to use Pacman and Flatpak

<h3> Pacman </h3>
- This command is for syncing databases and upgrading the whole system:
```bash
sudo pacman -Syu
```

- If you want to install an application or package (like Firefox, for example), use this command:
```bash
sudo pacman -S <package name>
```
where <package name> is the name of the package you want to install.
For instance, with firefox:  
```bash
sudo pacman -S firefox
```

- If you want to search for specific packages, use this command:
```bash
sudo pacman -Ss <package name>
```
where <package name> is the name of the package you want to search for.

- If you want to query installed packages, use this command:
```bash
sudo pacman -Qs <package name>
```
Alternatively, you can use the installed Infinity Linux tool 'Linux Ops Center' for updating the system, checking for updates, and package cache cleanup.


<h3> Flatpak </h3>
- This command is to add the Flatpak official remote app repo (Optional, only do this if Flatpak isn't finding any apps):
```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

- This command is to install apps from flatpak:
```bash
flatpak install <package name>
```
where <package name> in this context is in this format: org.mozilla.Firefox
for instance, to install Firefox (already installed by the system, just a reference):
```bash
flatpak install org.mozilla.Firefox
```

- To search for an app:
```bash
flatpak search <app name>
```

- To update flatpak in general:
```bash
flatpak update
```
## This should be enough for normal usage of the OS.

