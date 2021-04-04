# Magento2 Without Dummy
Install Magento CE Ver. 2.4.1 2020-09-25-04-08-02 in Windows XAMPP PHP 7.4

## Getting Started

### Basic Install

#### Donwload :
- Download [Magento Open Source 2](https://magento.com/tech-resources/download) without sample data
- Download [Elasticsearch](https://magentip.com/install-magento-2-on-localhost-xampp-elasticsearch) version 7.10.2 portable [mandatory]

#### Replace :
- Replace in [Gd2.php](https://magento.stackexchange.com/questions/311806/installation-at-51-module-magento-theme-error-in-magento-2)
- Replace in [PluginListGenerator.php](https://nwdthemes.com/2020/10/07/install-magento-2-4-on-windows-problem-solved/)
- Replace in [Validator.php](https://github.com/magento/magento2/issues/19480)

#### Command :
`note : instalation magento and create admin`
- `$ composer install`
- `$ php bin\magento setup:install --db-name=magento_demo` default => magento2 `note : after install environment has create in app/etc config.php [module] env.php [database]`
- `$ php bin\magento admin:user:create --admin-user=admin --admin-password=admin123 --admin-email=admin@admin.com --admin-firstname=admin --admin-lastname=admin`

#### Compile : [issue](https://community.magento.com/t5/Magento-2-x-Admin-Configuration/Magento-2-admin-page-load-but-login-window-is-not-show/m-p/49518#M822)
`note : for compile frontend`
- `$ php bin\magento setup:di:compile`
- `$ php bin\magento setup:upgrade`
- `$ php bin\magento setup:static-content:deploy`

### Issue
`note : error log in var/log/*`
- Xampp-control.exe run as Administrator
- `$ php bin/magento module:disable Magento_TwoFactorAuth`

<a href="REQUIREMENT.md">Requirement</a>

### Tutorial
- <a href="Tutorial-1.md">How to Create Module</a>.
- <a href="Tutorial-2.md">How to Create Controller</a>.
- <a href="Tutorial-3.md">CRUD Models</a>.
- <a href="Tutorial-4.md">Create View: Block, Layouts, Templates</a>.
- <a href="Tutorial-5.md">Create System.xml Configuration</a>.
- <a href="Tutorial-6.md">Create Admin Menu</a>.
- <a href="Tutorial-7.md">Create Admin Menu, ACL, and Grid</a>.
- <a href="Tutorial-8.md">Create Setup, Upgrade, Uninstall Script</a>.
- <a href="Tutorial-9.md">Events</a>.
- <a href="Tutorial-10.md">Plugin - Interceptor</a>.
- <a href="Tutorial-11.md">Indexing & Reindex</a>.
- <a href="Tutorial-12.md">Routing</a>.
- <a href="Tutorial-13.md">How to Add Command line in to Console CLI</a>.

### Uninstall
- `$ php bin\magento setup:uninstall`
