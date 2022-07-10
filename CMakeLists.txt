cmake_minimum_required(VERSION 3.5)

project(pisces-kwin-plugins)

set(PROJECT_NAME "pisces-kwin")

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

add_subdirectory(plugins)

install(FILES config/kglobalshortcutsrc DESTINATION /etc/xdg)
install(FILES config/kwinrc DESTINATION /etc/xdg)
install(FILES config/kwinrulesrc DESTINATION /etc/xdg)

install(DIRECTORY scripts/pisceslauncher DESTINATION /usr/share/kwin/scripts)
install(DIRECTORY scripts/pisces_squash DESTINATION /usr/share/kwin/effects)
install(DIRECTORY scripts/pisces_scale DESTINATION /usr/share/kwin/effects)
install(DIRECTORY scripts/pisces_popups DESTINATION /usr/share/kwin/effects)
install(DIRECTORY tabbox/pisces_thumbnail DESTINATION /usr/share/kwin/tabbox)
