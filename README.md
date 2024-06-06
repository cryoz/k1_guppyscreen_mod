# k1_guppyscreen_mod

Modded guppyscreen with changed temperature ranges: "190", "205", "220", "240", "260", "280", "320" with default 240

## Installing:

Required entware installed on K1/MAX printer for wget-ssl

```
opkg install wget-ssl && \
/opt/libexec/wget-ssl  -q https://github.com/cryoz/k1_guppyscreen_mod/raw/master/guppyscreen -O /usr/data/guppyscreen/guppyscreen.new && \
cp /usr/data/guppyscreen/guppyscreen /usr/data/guppyscreen/guppyscreen.bak && \
/etc/init.d/S99guppyscreen stop && \
mv /usr/data/guppyscreen/guppyscreen.new /usr/data/guppyscreen/guppyscreen && \
chmod +x /usr/data/guppyscreen/guppyscreen && \
/etc/init.d/S99guppyscreen start
```
