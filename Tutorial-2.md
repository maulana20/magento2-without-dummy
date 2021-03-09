# How to Create Controller

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/how-to-create-controllers-magento-2.html)
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
        - registration.php
```

Flush Magento Cache in `admin >> system >> cache management`

`note : if after flush magento blank, please run in bellow`

- `$ php bin/magento setup:upgrade`
- `$ php bin/magento setup:static-content:deploy`
- flush magento cache again
