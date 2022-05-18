Follow these steps to create Flatpak application of ClickHouse from binary:
1. Install Flatpak, if you don't have it (it is installed by default on Fedora and Manjaro):
    https://flatpak.org/setup/
2. Add Flathub repository:
```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
3. Install Freedesktop 21.08 runtime and SDK:
```
flatpak install flathub org.freedesktop.Platform//21.08 org.freedesktop.Sdk//21.08
```
4. Put ```clickhouse``` binary to the same directory as ```org.flatpak.ClickHouse.json```.
5. Build ClickHouse application with Flatpak:
```
flatpak-builder --user --install --force-clean build-dir org.flatpak.ClickHouse.json
```
6. Then you can run ClickHouse with:
```
flatpak run org.flatpak.ClickHouse
```
