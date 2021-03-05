# automate-wordpress-deployments

https://dzone.com/articles/how-to-automate-wordpress-deployments

1. Execute:
# navigate to theme directory
cd sage

# install php packages
composer validate
composer install
.........
2. Execute:yarn build:production
# navigate to theme directory
cd sage

# install packages
yarn

# Create production build
yarn build:production
.......

before this step-> create 1 click wordpress install in the choosen droplet, add ssh key, do ssh login, and notedown its ip address, type its ip address in the browser and verify that wordpress is working, do login, check all themes and plugins and switch themes , see website frontend
3.Upload files to ubuntu-s-4vcpu-8gb-blr1-01

ignore paths: 
.cache-loader/
node_modules/

source path: sage
Remote path: /var/www/html/wp-content/themes/sage
.......
4. Execute: sudo -u www-data -- wp theme activate sage/resources
sudo -u www-data -- wp theme activate sage/resources --path=/var/www/html/


