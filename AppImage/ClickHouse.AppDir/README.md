Follow these steps to create AppImage of ClickHouse:
1. Copy your ```./clickhouse``` binary to ```ClickHouse.AppDir/usr/bin```.
2. Give execute permissions to ```AppRun``` and ```clickhouse.desktop```:
```
chmod +x ClickHouse.AppDir/AppRun
chmod +x ClickHouse.AppDir/clickhouse.desktop
```
3. Get AppImageTool with:
```
wget "https://github.com/AppImage/AppImageKit/releases/download/continuous/appimagetool-x86_64.AppImage"
chmod a+x appimagetool-x86_64.AppImage
```
4. Build the AppImage with:
```
ARCH=x86_64 ./appimagetool-x86_64.AppImage ClickHouse.AppDir 
```
5. After that, you should get executable ```clickhouse-x86_64.AppImage```.
