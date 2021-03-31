# Create Setup, Upgrade, Uninstall Script

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/magento-2-how-to-create-sql-setup-script.html)
`note : `  `` as directory
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `etc`
          - module.xml
        - `Setup`
          - InstallSchema.php
          - UpgradeSchema.php
          - InstallData.php
          - UpgradeData.php
          - Uninstall.php
        - `Model`
          - `ResourceModel`
            - `Post`
              - Collection.php
            - Post.php
          - Post.php
        - registration.php
```

Compile : 

- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:static-content:deploy`
