# composer-versions-check

A plugin for Composer. It warns user for outdated packages from last major versions after update command.

[![CI](https://github.com/dereuromark/composer-versions-check/actions/workflows/ci.yml/badge.svg)](https://github.com/dereuromark/composer-versions-check/actions/workflows/ci.yml)
[![Latest Stable Version](https://poser.pugx.org/dereuromark/composer-versions-check/v/stable)](https://packagist.org/packages/dereuromark/composer-versions-check)
[![License](https://poser.pugx.org/dereuromark/composer-versions-check/license)](https://packagist.org/packages/dereuromark/composer-versions-check)
[![Total Downloads](https://poser.pugx.org/dereuromark/composer-versions-check/downloads)](https://packagist.org/packages/dereuromark/composer-versions-check)
[![Monthly Downloads](https://poser.pugx.org/dereuromark/composer-versions-check/d/monthly)](https://packagist.org/packages/dereuromark/composer-versions-check)
[![Daily Downloads](https://poser.pugx.org/dereuromark/composer-versions-check/d/daily)](https://packagist.org/packages/dereuromark/composer-versions-check)

![composer-versions-check_demo](https://cloud.githubusercontent.com/assets/1698357/14637529/2e32a778-0632-11e6-99c7-0e1c284a7436.gif)

<sup>Screencast provided by [Silentcast](https://github.com/colinkeenan/silentcast).</sup>

## Installation

You can install it either globally (recommended):

```bash
composer global require dereuromark/composer-versions-check
```

or locally (as require-dev dependency then):

```bash
composer require --dev dereuromark/composer-versions-check
```

## Usage

That's it! Composer will enable automatically the plugin as soon it's installed.

Just run `composer update` command to see the plugin working.

## Configuration

You can configure the plugin via the [`COMPOSER_HOME/config.json`](https://getcomposer.org/doc/03-cli.md#composer-home) file. Here is the default one:

```json
{
    "config": {
        "dereuromark-composer-versions-check": {
            "show-links": false
        }
    }
}
```

* `show-links`: Shows outdated package links. Set to `true` to get a larger output, like the demo.
