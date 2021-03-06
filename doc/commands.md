# Commands

## Installation
GrumPHP comes shipped with a configuration tool. Run following command to create a basic configuration file:

```sh
php ./vendor/bin/grumphp configure
```

This command gets invoked during installation.
It wil not ask you for anything, but it will try to guess the best possible configuration.

To enable or disable GrumPHP, you can run one of the following commands:
 
```sh
php ./vendor/bin/grumphp git:init
php ./vendor/bin/grumphp git:deinit
```

The `git:init` is triggered by the composer plugin during installation.

## Git hooks

GrumPHP will be triggered with GIT hooks. However, you can run following commands:

```sh
php ./vendor/bin/grumphp git:pre-commit
php ./vendor/bin/grumphp git:commit-msg
```

## Run

If you want to run the tests on the full codebase, you can run the command:

```sh
php ./vendor/bin/grumphp run
```

This command can also be used for continious integration.
