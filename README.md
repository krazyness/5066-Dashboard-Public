mkdir -p ~/.config/autostart

vim ~/.config/autostart/kiosk.desktop

sudo apt install -y fonts-noto-color-emoji

**Insert:**

[Desktop Entry]
Type=Application

Name=Kiosk Browser

Exec=chromium --enable-gpu-rasterization --enable-zero-copy --ignore-gpu-blocklist --disable-software-rasterizer --disable-extensions --disable-sync --disable-translate --disable-features=TranslateUI --noerrdialogs --disable-infobars --kiosk --incognito file:///home/hornet/frc_dashboard/index.html

Hidden=false

NoDisplay=false

X-GNOME-Autostart-enabled=true


Then run:

sudo mv /usr/share/dbus-1/services/org.freedesktop.secrets.service ~/
