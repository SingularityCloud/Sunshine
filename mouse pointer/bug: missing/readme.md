# Problem:
bug:
- https://github.com/LizardByte/Sunshine/issues/93
- https://github.com/LizardByte/Sunshine/pull/1078

sch: https://www.google.com/search?q=lizardbyte+sunshine+mouse+pointer

# Solution
## use Xorg
Temporary, **works!**:
Logout and login to Xorg instead.

- https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1483938743

## Wayland
Gnome:
https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1374964995

KDE:
- https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1483941690
- https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1377858388
  - https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1383037304
  - https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1383309264

```
dir="~/.config/environment.d/"
mkdir -p $dir ; cd $dir
echo "KWIN_FORCE_SW_CURSOR=1" > mouse.conf
```
OR:
```
dir="~/environment.d/"
mkdir -p $dir ; cd $dir
echo "export KWIN_FORCE_SW_CURSOR=1" > 10-kwin-force-sw-cursor=1
```

# relation: RustDesk
https://github.com/LizardByte/Sunshine/issues/93#issuecomment-1483941690
