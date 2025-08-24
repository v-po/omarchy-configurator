# Omarchy Configurator

This is a minimal frontend for archinstall, which collects the user information and disk choice to produce the `user_configuration.json`, `user_credentials.json`, `user_email_address.txt`, and `user_full_name.txt` files that are then used by [the omarchy-iso setup](https://github.com/omacom-io/omarchy-iso) to start a preconfigured archinstall.

This repository is pulled into the omarchy-iso-make process at runtime.

## Testing

You can test this script in dry mode like:
- Without any network detection: `NETWORK_NOT_NEEDED=1 ./configurator dry`.
- Force wifi selection: `WIFI_NEEDED=1 ./configurator dry`.
- Normal network detection: `./configurator dry`.
