# Instructions
## Clone the repository
```
git clone git@github.com:penleychan/keyball61-maps.git keyball
```

## Clone qmk firmware
```
git clone https://github.com/idank/qmk_firmware.git --depth 1 --recurse-submodules --shallow-submodules -b holykeebs-master qmk
```

## Create sym link
```
cd qmk/keyboards
rm -rf keyball/
ln -s ../../keyball/qmk_firmware/keyboards/keyball keyball
```

## Build
```
make keyball/keyball61:default
```

## Useful commands
```
find . -name "*:Zone.Identifier" -type f -delete
```

# Information 
[QMK KeyCodes](https://github.com/qmk/qmk_firmware/blob/master/docs/keycodes.md)
[Special Key](https://github.com/Yowkees/keyball/blob/main/qmk_firmware/keyboards/keyball/lib/keyball/keycodes.md)

