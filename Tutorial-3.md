# CRUD Models

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/how-to-create-crud-model-magento-2.html)
`note : `  `` as directory
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `Controller`
          - `Index`
            - Index.php
        - `etc`
          - `frontend`
            - routes.xml
          - module.xml
        - `Setup`
          - InstallSchema.php
          - UpgradeSchema.php
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

Note :

- In case `\Mageplaza\HelloWorld\Model\PostFactory` will automatically generate the Factory class in the `var/generation`
- In `module.xml` file, we changed the attribute to 1.1.0 greater than `setup_version`

