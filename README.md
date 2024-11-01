# WP BOOKING PLUGIN

* go to http://127.0.0.1:8080/

## Tests
* see test folder for detailed wp setup in docker container.
* install wp cli in container:
```bash
curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
chmod +x wp-cli.phar
mv wp-cli.phar /usr/local/bin/wp
```
* example usage of wp cli:
```bash
# install plugin
wp plugin install wp-content/my-plugin.zip

# activate plugin
wp plugin activate woocommerce 

# list all installed plugins
wp plugin list

# delete plugin
wp plugin delete woocommerce --allow-root
```