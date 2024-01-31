# MazePress - Private Packagist
A self-hosted static Composer repository generator for Private Packagist based on [Satis](https://github.com/composer/satis).

### Available Packages
The following are the available packages.

| Package | Description |
| --- | --- |
| `mazepress/core` | A custom framework library for WordPress plugin and theme development. |
| `mazepress/forms` | A package library for creating HTML forms |

## Development
Clone or fork the repository and install the dependencies by running the following commands.

Install the [Composer](https://getcomposer.org/) dependency packages.
```Shell
composer install
```

Build all the private packages using [Satis](https://nodejs.org) dependency packages.
```Shell
composer run build
```
### Dependencies
- [Composer](https://getcomposer.org/) version: 2.0 or higher

## Usage
In your projects, add your own Composer repository using the `https://mazepress.github.io/packagist` as URL, then you can require your private packages and everything should work smoothly.

Read more detailed instructions in the [documentation](https://getcomposer.org/doc/articles/handling-private-packages.md).

### Example
composer.json
```YAML
{
    "name": "mycompany/mycompany-project",
    "require": {
        "mycompany/privaterepo": "^1.0"
    },
    "repositories": [
        {
            "type": "composer",
            "url": "https://mazepress.github.io/packagist"
        }
    ]
}
```

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE.md) for more information.
