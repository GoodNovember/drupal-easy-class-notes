# DDEV Install mode

The magic invocation for a new DDEV instance is `ddev config`

## Before Drupal Install

```
mkdir garbage
cd garbage
ddev config --project-type php
```

## Drupal Install

```
ddev composer create drupal-composer/drupal-project:8.x-dev --stability dev --no-interaction --prefer-dist
```

## Post Drupal Install
```
ddev config --project-type drupal8
ddev restart
```

## When Ready:
```
ddev start
```

## Troubleshooting

### The console complains about incorrect username and password when talking about `ddev-ssh-agent`

1. Logout and back in from the Docker App itself. 
2. run `ddev auth ssh` and see if it is sucessful.
3. ???
4. PROFIT!