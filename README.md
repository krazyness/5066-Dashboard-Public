mkdir -p ~/.config/autostart
vim ~/.config/autostart/kiosk.desktop

[Desktop Entry]
Type=Application
Name=Kiosk Browser
Exec=chromium-browser --noerrdialogs --disable-infobars --kiosk --incognito file:///full/path/to/your/file.html
Hidden=false
NoDisplay=false
X-GNOME-Autostart-enabled=true
