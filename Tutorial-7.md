# Create Admin Menu, ACL, and Grid

## Getting Started

### Directory File : [menu](https://www.mageplaza.com/magento-2-module-development/create-admin-menu-magento-2.html) [acl](https://www.mageplaza.com/magento-2-module-development/magento-2-acl-access-control-lists.html) [grid](https://www.mageplaza.com/magento-2-module-development/create-admin-grid-magento-2.html)
`note : `  `` as directory
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `Controller`
          - `Adminhtml`
            - `Post`
              - Index.php
        - `etc`
          - `adminhtml`
            - routes.xml
            - menu.xml
            - system.xml
          - module.xml
          - config.xml
          - acl.xml
          - di.xml
        - `Setup`
          - InstallSchema.php
          - UpgradeSchema.php
        - `Model`
          - `ResourceModel`
            - `Post`
              - Collection.php
            - Post.php
          - Post.php
        - `view`
          - `adminhtml`
            - `layout`
              - mageplaza_helloworld_post_index.xml
            - `ui_component`
              - mageplaza_helloworld_post_listing.xml
        - registration.php
```

Compile : 

- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:static-content:deploy`

Flush Magento Cache in `admin >> system >> cache management`
