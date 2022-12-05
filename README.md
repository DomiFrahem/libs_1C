# lib_1C_8.3.17-19

## load libs

```
git clone http://tj.kbsu.ru/AlexSidorov/install_1C_8.3.17.git
```

## copy all libs
### 1C_8.3.17
```
sudo cp install_1C_8.3.19/*so* /opt/1C/v8.3/x86_64/ 
```
### 1C_8.3.19
```
sudo cp install_1C_8.3.19/*so* /opt/1cv8/x86_64/8.3.19.1723/
```

## create links
### 1C_8.3.17
```
sudo ln -s /opt/1C/v8.3/x86_64/libicui18n.so.60.3 /opt/1C/v8.3/x86_64/libicui18n.so.60
sudo ln -s /opt/1C/v8.3/x86_64/libicuuc.so.60.3 /opt/1C/v8.3/x86_64/libicuuc.so.60
sudo ln -s /opt/1C/v8.3/x86_64/libicudata.so.60.3 /opt/1C/v8.3/x86_64/libicudata.so.60
sudo ln -s /opt/1C/v8.3/x86_64/libjavascriptcoregtk-3.0.so.0.16.19 /opt/1C/v8.3/x86_64/libjavascriptcoregtk-3.0.so.0
sudo ln -s /opt/1C/v8.3/x86_64/libwebkitgtk-3.0.so.0.22.17 /opt/1C/v8.3/x86_64/libwebkitgtk-3.0.so.0
```
### 1C_8.3.19
```
sudo ln -s /opt/1cv8/x86_64/8.3.19.1723/libicui18n.so.60.3 /opt/1cv8/x86_64/8.3.19.1723/libicui18n.so.60
sudo ln -s /opt/1cv8/x86_64/8.3.19.1723/libicuuc.so.60.3 /opt/1cv8/x86_64/8.3.19.1723/libicuuc.so.60
sudo ln -s /opt/1cv8/x86_64/8.3.19.1723/libicudata.so.60.3 /opt/1cv8/x86_64/8.3.19.1723/libicudata.so.60
sudo ln -s /opt/1cv8/x86_64/8.3.19.1723/libjavascriptcoregtk-3.0.so.0.16.19 /opt/1cv8/x86_64/8.3.19.1723/libjavascriptcoregtk-3.0.so.0
sudo ln -s /opt/1cv8/x86_64/8.3.19.1723/libwebkitgtk-3.0.so.0.22.17 /opt/1cv8/x86_64/8.3.19.1723/libwebkitgtk-3.0.so.0
```

## delete libstdc++.so.6

Не разбирался, но эта штука просто мешает

```
sudo rm /opt/1C/v8.3/x86_64/libstdc++.so.6
```

## Конец
После этого все запускается, ну по крайней мере у меня.<br />
Проверял на <b>Fedora 36-37</b>

