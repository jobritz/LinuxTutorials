# deskshcut
Create runnable desktop shortcut in linux

# Step 1:
Create a .sh-file
```bash
nano file.sh
```

and write the command line you need to start the programm
(Example: Xampp)
```bash
sudo /opt/lampp/manager-linus-x64.run
```

then save your file.

# Step 2:
Add a tag to make file runnable
```bash
chmod +x file.sh
```

# Step 3:
Create a .desktop-file:
```bash
sudo nano file.desktop
```

and copy this text in your file:
```bash
[Desktop Entry]
Version=1.0
Exec=/destination of your sh file/filname.sh
Name= --Anything--
GenericName= --Anything--
Comment= --Anything--
Encoding=UTF-8
Terminal=true
Type=Application
Categories=Application
```

Save this file anywhere now, you need to move it via terminal.

# Step 4:
Add a tag to make file runable

```bash
chmod +x file.desktop
```

# Step 5:
then move the .desktop file:

```bash
sudo mv file.desktop /usr/share/applications
```

Now you should be able to find this shortcut in your Applications
