Follow these steps to create Snap of ClickHouse:
1. Install Snap, if you don't have it (it is installed by default on Ubuntu and Manjaro):
    https://snapcraft.io/docs/installing-snapd
2. Install snapcraft for building Snaps:
```
sudo snap install snapcraft --classic
```
3. Run ```snapcraft``` in the directory with ```snapcraft.yaml```.
4. You will get ```clickhouse_*.snap``` file, which you can then install locally:
```
sudo snap install clickhouse_*.snap --devmode --dangerous
```
5. Now you can run ClickHouse with just ```clickhouse``` command.
