# Magento2 Without Dummy
Install Magento CE Ver. 2.4.1 2020-09-25-04-08-02 in Windows XAMPP PHP 7.4

## Getting Started

### Basic Install

Donwload :
1.  Download Magento Open Source 2 without sample data {link](https://magento.com/tech-resources/download)
2.  Download elasticsearch version 7.10.2 portable [mandatory] [link](https://magentip.com/install-magento-2-on-localhost-xampp-elasticsearch)

Replace :
3.  Replace in Gd2.php [link](https://magento.stackexchange.com/questions/311806/installation-at-51-module-magento-theme-error-in-magento-2)
4.  Replace in PluginListGenerator.php [link](https://nwdthemes.com/2020/10/07/install-magento-2-4-on-windows-problem-solved/)
5.  Replace in Validator.php [link](https://github.com/magento/magento2/issues/19480)

Command :
`note : instalation magento and create admin`
6.  `$ composer install`
7.  `$ php bin\magento setup:install --db-name=magento_demo` default => magento2 `note : after install environment has create in app/etc config.php (module) env.php (database)`
8.  `$ php bin\magento admin:user:create --admin-user=admin --admin-password=admin123 --admin-email=admin@admin.com --admin-firstname=admin --admin-lastname=admin`

Compile : [issue](https://community.magento.com/t5/Magento-2-x-Admin-Configuration/Magento-2-admin-page-load-but-login-window-is-not-show/m-p/49518#M822)
`note : for compile frontend`
9.  `$ php bin\magento setup:upgrade`
10. `$ php bin\magento setup:di:compile`
11. `$ php bin\magento setup:static-content:deploy`

### Issue
`note : error log in var/log/*`
1.  xampp-control.exe run as Administrator
2.  `$ php bin/magento module:disable Magento_TwoFactorAuth`
