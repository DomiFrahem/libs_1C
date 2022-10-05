# lib_1C_8.3.17

## load libs

```
git clone http://tj.kbsu.ru/AlexSidorov/install_1C_8.3.17.git
```

## copy all libs
```
# cp install_1C_8.3.17/*so* /opt/1C/v8.3/x86_64/ 
```

## create links
```
# ln -s /opt/1C/v8.3/x86_64/libjavascriptcoregtk-3.0.so.0.16.19 /opt/1C/v8.3/x86_64/libjavascriptcoregtk-3.0.so.0
# ln -s /opt/1C/v8.3/x86_64/libwebkitgtk-3.0.so.0.22.17 /opt/1C/v8.3/x86_64/libwebkitgtk-3.0.so.0
```

## delete libstdc++.so.6

Не разбирался, но эта штука просто мешает

```
# rm /opt/1C/v8.3/x86_64/libstdc++.so.6
```

## Конец
После этого все запускается, ну по крайней мере у меня.<br />
У меня на данный момент стоит <b>Fedora 37</b>

