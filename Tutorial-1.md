# Simple Hello Word Module

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/)
`note : `directory``
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `Controller`
          - `Index`
            - Test.php
        - `etc`
          - `frontend`
            - routes.xml
          - module.xml
        - registration.php
```

### Compile :
`note : check module after create`
- `$ php bin/magento module:status` 
- `$ php bin/magento module:enable Mageplaza_HelloWorld`

`note : generate in frontend`
- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:static-content:deploy` [optional]
