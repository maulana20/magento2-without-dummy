# Create System.xml Configuration

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/create-system-xml-configuration-magento-2.html)
`note : `  `` as directory
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `Controller`
          - `Index`
            - Config.php
        - `Helper`
          - Data.php
        - `etc`
          - `adminhtml`
            - system.xml
          - module.xml
          - config.xml
        - registration.php
```

Compile : 

Flush Magento Cache in `admin >> system >> cache management`

- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:static-content:deploy`
