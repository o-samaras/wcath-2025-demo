# Modern WordPress Development with Composer
This repository acts as a quick demo or blueprint on how to utilise 
Composer to build and maintain WordPress projects.
This was created to accompany my talk on [WordCamp Athens 2025](https://athens.wordcamp.org/2025/session/modern-wordpress-development-with-composer/).

## What is included
This repository includes by default the following files (in order of importance):

- `composer.json`:
The heart and soul of this repository 😁 This is the main Composer configuration file, containing the
project's dependencies, meta information, extra configuration and scripts. It is accompanied by the automatically
generated `composer.lock`.

- `index.php`
This acts as the entry point for the WordPress application. The only thing this file does, is to include the 
WordPress's default `index.php`. This is needed, because the default WordPress's `index.php` is located inside
the package's installation directory (by default `wordpress` in this demo `wp`) and not in the project's root
directory.

- `.gitignore`
This file is neither directly used nor required for the project's functionality. It contains files that will be
installed by Composer, but shouldn't be included in the VCS (Version Control Systems - e.g. GIT).

- `.ddev`
You can freely ignore this directory completely. It contains configuration for DDEV, a tool used for creating
and managing local development environments based on Docker. If you want to use it though, you can found more
information on how to install and use it in the links provided below.

## How to use this
1. Clone this repository.
2. `cd` into the directory you cloned the repository.
3. Execute the command `composer install`
4. Open your browser and navigate to the same directory (the one you cloned the repository into).

### Prerequisites
For this to work as expected, the following are required:
1. Web server (Apache, NGINX etc.)
2. PHP
3. MySQL/MariaDB
4. Composer

If you decide to use the included DDEV tool, then all of the above are automatically included
and there's no need for you to take further actions.

## Resources
- [Composer](http://getcomposer.org/)
- [DDEV](https://docs.ddev.com/en/stable/)
- [Using Composer with DDEV](https://ddev.com/blog/getting-started-with-ddev-and-composer/)
- [How to clone a GitHub repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) 
