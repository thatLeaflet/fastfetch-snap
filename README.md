Note: This is an unofficial repackaging and is not endorsed by the upstream project. The upstream fastfetch project can be found [here](https://github.com/fastfetch-cli/fastfetch).

## Want to build the snap yourself?

Before you begin
- Ensure you have snapd installed
- Ensure you have git installed

How to set up snapcraft
- Install snapcraft: run `sudo snap install snapcraft --classic`
- Install lxd: run `sudo snap install lxd`
- Add your user to the lxd group: run `sudo usermod -aG lxd $USER`
- Reboot your computer
- Configure lxd: run `lxd init --minimal`

How to build the snap
- Enter a nice working directory (e.g. ~/projects)
- Download repo: run `git clone https://github.com/thatLeaflet/fastfetch-snap.git && cd ./fastfetch-snap`
- Build the snap: run `snapcraft`
- Install the snap:
  - amd64: run `sudo snap install --dangerous --classic ./fastfetch_*_amd64.snap`
  - arm64: run `sudo snap install --dangerous --classic ./fastfetch_*_arm64.snap`
