# How to Add Command line in to Console CLI

## Getting Started

### Directory File : [tutorial](https://www.mageplaza.com/magento-2-module-development/magento-2-how-to-add-command-line-console-cli.html)
`note : `  `` as directory
```bash
- `app`
  - `code`
    - `Mageplaza`
      - `HelloWord`
        - `Console`
          - Sayhello.php
        - `etc`
          - module.xml
          - di.xml
        - registration.php
```

Compile : 

Flush Magento Cache in `admin >> system >> cache management` or `php bin\magento cache:flush config`

Command :

- `$ php bin\magento example:sayhello --help`
- `$ php bin\magento example:sayhello --name=test`
