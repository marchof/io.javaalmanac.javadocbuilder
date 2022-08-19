# OpenJDK JavaDoc Builds

There are no downloadable JavaDoc builds for the OpenJDK releases. The GitHub
actions in this repository are able to build JavaDoc for all OpenJDK releases
since OpenJDK 8.

## How does it work?

Building OpenJDK basically means installing several prerequisites and kicking
off the documentation build. To make it look nicer we add
[the missing JavaDoc fonts](https://github.com/marchof/the-missing-javadoc-fonts).
These steps are performed as GitHub actions.

This repository contains a [shared build action](.github/workflows/javadoc.yml)
in the main branch and release specific configurations
[individual branches](../../branches).

## Where can I download the JavaDoc?

Not here. While OpenJDK source is published under the GPL the JavaDoc build adds
a link to Oracle's [documentation redistribution policy](https://www.oracle.com/technetwork/java/redist-137594.html)
which does not allow re-distribution. You may clone this repository and build
the JavaDoc yourself on your own risk.

## License

The scripts are provided "as is" under the [MIT License](LICENSE.md), without
warranty of any kind.