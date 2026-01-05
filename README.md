mkdir -p ~/.config/autostart

vim ~/.config/autostart/kiosk.desktop

**Insert:**

[Desktop Entry]
Type=Application

Name=Kiosk Browser

Exec=chromium --noerrdialogs --disable-infobars --kiosk --incognito file:///home/hornet/frc_dashboard/index.html

Hidden=false

NoDisplay=false

X-GNOME-Autostart-enabled=true


Then run:

sudo mv /usr/share/dbus-1/services/org.freedesktop.secrets.service ~/
