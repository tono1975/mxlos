mxlos.com
--

This is a Composer-based installer for the [Lightning](https://www.drupal.org/project/lightning) Drupal distribution. Welcome to the future!

## Project setup
```
# Fork repository
https://github.com/octahedroid/mxlos/fork

# Clone repository
git clone git@github.com:USER_NAME/mxlos.git

# Copy .env file
cp .env.dist .env

# Add hostname entry in your /etc/hosts file
127.0.0.1    mxlos.develop
```

## Sync Project
```
# Switch develop branch
git checkout develop

# Fetch latest changes
git fetch upstream

# Merge changes locally
git merge upstream/develop

# Sync forked repo 
git push origin/develop

# Download new dependencies
ahoy composer install

# Build Drupal site
ahoy drupal build:develop
```

## Download new dependencies 
```
ahoy composer require drupal/MODULE_NAME
```

## Export Configuration
```
ahoy drupal config_split:export --no-interaction
```
