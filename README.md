# Drupal Open AI

A demo project template to POC AI-related things with Drupal.

## Requirement

Install [Lando](https://lando.dev/) on your machine.

## Getting started

```bash
git clone https://github.com/MatthieuScarset/drupal-openai.git
cd drupal-openai
rm -rf .git/
cp .env.example .env
git init && git add . && git commit -m "chore: Init project" && git push
lando start
lando composer install -o
lando drush site:install --existing-config -y
lando drush user:password admin admin
lando drush user:login
```

Get to work now!