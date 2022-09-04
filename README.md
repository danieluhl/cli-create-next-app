oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g cli-create-next-app
$ cli-create-next-app COMMAND
running command...
$ cli-create-next-app (--version)
cli-create-next-app/0.0.0 darwin-arm64 node-v18.6.0
$ cli-create-next-app --help [COMMAND]
USAGE
  $ cli-create-next-app COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`cli-create-next-app hello PERSON`](#cli-create-next-app-hello-person)
* [`cli-create-next-app hello world`](#cli-create-next-app-hello-world)
* [`cli-create-next-app help [COMMAND]`](#cli-create-next-app-help-command)
* [`cli-create-next-app plugins`](#cli-create-next-app-plugins)
* [`cli-create-next-app plugins:install PLUGIN...`](#cli-create-next-app-pluginsinstall-plugin)
* [`cli-create-next-app plugins:inspect PLUGIN...`](#cli-create-next-app-pluginsinspect-plugin)
* [`cli-create-next-app plugins:install PLUGIN...`](#cli-create-next-app-pluginsinstall-plugin-1)
* [`cli-create-next-app plugins:link PLUGIN`](#cli-create-next-app-pluginslink-plugin)
* [`cli-create-next-app plugins:uninstall PLUGIN...`](#cli-create-next-app-pluginsuninstall-plugin)
* [`cli-create-next-app plugins:uninstall PLUGIN...`](#cli-create-next-app-pluginsuninstall-plugin-1)
* [`cli-create-next-app plugins:uninstall PLUGIN...`](#cli-create-next-app-pluginsuninstall-plugin-2)
* [`cli-create-next-app plugins update`](#cli-create-next-app-plugins-update)

## `cli-create-next-app hello PERSON`

Say hello

```
USAGE
  $ cli-create-next-app hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Whom is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/learning/cli-create-next-app/blob/v0.0.0/dist/commands/hello/index.ts)_

## `cli-create-next-app hello world`

Say hello world

```
USAGE
  $ cli-create-next-app hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oex hello world
  hello world! (./src/commands/hello/world.ts)
```

## `cli-create-next-app help [COMMAND]`

Display help for cli-create-next-app.

```
USAGE
  $ cli-create-next-app help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for cli-create-next-app.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `cli-create-next-app plugins`

List installed plugins.

```
USAGE
  $ cli-create-next-app plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ cli-create-next-app plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `cli-create-next-app plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ cli-create-next-app plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ cli-create-next-app plugins add

EXAMPLES
  $ cli-create-next-app plugins:install myplugin 

  $ cli-create-next-app plugins:install https://github.com/someuser/someplugin

  $ cli-create-next-app plugins:install someuser/someplugin
```

## `cli-create-next-app plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ cli-create-next-app plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ cli-create-next-app plugins:inspect myplugin
```

## `cli-create-next-app plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ cli-create-next-app plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ cli-create-next-app plugins add

EXAMPLES
  $ cli-create-next-app plugins:install myplugin 

  $ cli-create-next-app plugins:install https://github.com/someuser/someplugin

  $ cli-create-next-app plugins:install someuser/someplugin
```

## `cli-create-next-app plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ cli-create-next-app plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ cli-create-next-app plugins:link myplugin
```

## `cli-create-next-app plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cli-create-next-app plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-create-next-app plugins unlink
  $ cli-create-next-app plugins remove
```

## `cli-create-next-app plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cli-create-next-app plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-create-next-app plugins unlink
  $ cli-create-next-app plugins remove
```

## `cli-create-next-app plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ cli-create-next-app plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-create-next-app plugins unlink
  $ cli-create-next-app plugins remove
```

## `cli-create-next-app plugins update`

Update installed plugins.

```
USAGE
  $ cli-create-next-app plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
