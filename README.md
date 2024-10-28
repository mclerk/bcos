# bcos (Bootc Operating System) image

This repository is based on [ublue-os/image-template](https://github.com/ublue-os/image-template).

Currently built on top of [Bluefin](https://projectbluefin.io/) with customizations.

## TODO

- [ ] Add flatpaks
- [ ] Edit Default Settings
- [ ] Create iso for installion
- [ ] Multiple Image creation
  - [ ] Nvidia Support
  - [ ] Rasberry Pi support (Targeting Pi 5)
- [ ] Remove Homebrew
- [ ] Create & add my own custom rpm repo, with custom builds

## Installation

This image is meant for x86_64 with AMD & Intel Graphics. (Nvidia & Pi Image coming soon)

I don't have iso creation in my builds currently but coming soon.

### 1. Reset rpm-ostree

```bash
rpm-ostree reset
```
### 2. Rebase rpm-ostree

```bash
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/mclerk/bcos:latest
```

