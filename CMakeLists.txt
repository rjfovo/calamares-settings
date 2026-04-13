cmake_minimum_required(VERSION 3.5)

project(calamares-settings)

# Install settings.conf
install(FILES cutefish_config/settings.conf DESTINATION /etc/calamares)

# Install branding files
install(DIRECTORY cutefish_config/branding/cutefishos
        DESTINATION /usr/share/calamares/branding
        USE_SOURCE_PERMISSIONS)

# Install module configuration files
install(DIRECTORY cutefish_config/modules
        DESTINATION /etc/calamares
        USE_SOURCE_PERMISSIONS)
