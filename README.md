# Cirily KWin Plugins

## Dependencies (For Arch)
```bash
sudo pacman -S extra-cmake-modules qt5-base qt5-declarative kconfig kdecoration kguiaddons kcoreaddons kconfigwidgets kwindowsystem kwayland kwin
```
## Build

```bash
git clone https://github.com/cirily/kwin-plugins.git
cd kwin-plugins
mkdir build
cd build
cmake ..
make
sudo make install
```

## License

pisces-kwin-plugins is licensed under GPLv3.
