# Create Controller View

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
        - `view`
          - `frontend`
            - `layout`
              - helloword_index_index.xml
            - `templates`
              - index.phtml
        - `Block`
          - Index.php
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

`note : in case \Mageplaza\HelloWorld\Model\PostFactory will automatically generate the Factory class in the var/generation after run command php bin\magento setup:di:compile`

- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:di:compile`
- `$ php bin/magento setup:static-content:deploy`
- flush magento cache `admin >> system >> cache management` [optional]
