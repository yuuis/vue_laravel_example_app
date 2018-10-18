# Vue.js + Laravel5.5 sample app

## operations
**※ you have to install `Composer`.**

```bash:console
# clone project
git clone https://github.com/tosite0345/vue.js-laravel-sample.git

# start VM
composer install
./vendor/bin/homestead make
vagrant up

vagrant ssh
cd 'project-root'
composer install
php artisan config:cache

# create sample User
# mail : homestead@sample.com
# pass : secret
php artisan migrate
php artisan db:seed

# install passport
php artisan passport:install
```