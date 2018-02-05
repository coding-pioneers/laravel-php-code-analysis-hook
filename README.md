# laravel-php-code-analysis-hook
A GIT pre-commit hook for running php code sniffer, php mess detector and phpunit before a commit can be accepted.

## Installation
Add the repository to your composer.json

```
"repositories": [
     {
         "url": "https://github.com/coding-pioneers/laravel-php-code-analysis-hook.git",
         "type": "git"
     } ]
```
Add the following line to your composer.json to the require-dev-section
```
"coding-pioneers/laravel-php-code-analysis-hook": "@dev"
```
Then run `composer update`

To add the new git-hook to your repository run the following command
```
vendor/bin/symlink-git-hooks-to-hub  
```
Now your source code is being checked before the commit.

##Uninstall
Remove the link to the pre-commit-hook with the following command
```
vendor/bin/remove-git-hook
```
Then remove the following line from your composer.json
```
"coding-pioneers/laravel-php-code-analysis-hook": "@dev"
```
Then run `composer update`