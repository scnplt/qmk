# Setup

```bash
git clone https://github.com/scnplt/qmk.git && cd qmk
git submodule update --init --recursive --depth 1

# https://qmk.fm/guide
qmk setup -H "$(pwd)/vial-qmk"
mkdir vial-qmk/keyboards/scnplt
```

# Flash

```bash
cp -r lily58 vial-qmk/keyboards/scnplt

# For left side
qmk flash -kb scnplt/lily58 -km vial -bl uf2-split-left

# For right side
qmk flash -kb scnplt/lily58 -km vial -bl uf2-split-right
```
