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

Translations can be done via crowdin (at the moment ``.adoc`` are not fully supported). All gradle tasks use the offical ``crodwin-cli`` jar file to
interact with crowdin.

* ``crowdinHelp`` display help for crodwin-cli
