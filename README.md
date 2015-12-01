# turbulent-octo-squeegee

This is an Asciidoctor sample project supporting translation via crowdin. Everything can be automated using different gradle tasks.

# Requirements

* Installed Java SDK (tested against latest JDK8)

# Tasks

* ``htmlGerman`` creates the german html documentation
* ``pdfGerman`` created the german PDF documentation
* ``htmlEnglish`` creates the english html documentation
* ``pdfEnglish`` created the english PDF documentation

# Usage

To generate german html and pdf just execute ``./gradlew``, both will be executed as default tasks. For other tasks
just execute ``./gradlew htmlEnglish`` for example.

# Crowdin integration

**At the moment crowdin does not support .adoc files**, but [support is comming soon](https://twitter.com/crowdin/status/669975732622372864).

Translations can be done via crowdin (at the moment ``.adoc`` are not fully supported). All gradle tasks use the offical ``crodwin-cli`` jar file to
interact with crowdin.

## Setup

You just need to add a file called ``crodwin-account.yaml``. It must contain your crowdin api key.

```yaml
api_key: YOUR_API_KEY
```

In ``crowdin-config-yaml`` you just need to replace the ``project_identifier`` with your project. Depending on your file structure you may need to add additional source files
in this config file.

## Usage

* ``crowdinHelp`` display help for crodwin-cli
