# module_updates_overview

Provides a copy/paste friendly overview of the modules in need of updates.

Used to coordinate broad heavy module update tasks, deviding the updates into
groups making it more test-able and safe to update by groups.

## Installation

Enable the module

### Composer
```
        "drupal/module_updates_overview": "1.x-dev",
.
.
.
        {
            "type": "package",
            "package": {
                "name": "drupal/module_updates_overview",
                "version": "1.x-dev",
                "type": "drupal-module",
                "source": {
                    "url": "https://github.com/adaptdk/module_updates_overview.git",
                    "type": "git",
                    "reference": "refs/heads/7.x-1.x"
                }
            }
        }
```

## Usage

```
# Enable this module
$ drush en module_updates_overview

# Update the status of the modules.
$ drush @astra.dev pm-updatestatus
```

Visit /admin/module_updates_overview and the list is copy/paste ready for a
google sheet, coordinating the creation of tasks and progress.
