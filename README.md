<p align='center'>
<img src="https://github.com/barbu-it/paasify/raw/main/logo/paasify_collection.svg" alt="Paasify Collection">
</p>

# Paasify Collection: official

This collection only contains verified publisher images.

## Quickstart

In your `paasify.yml` configuration, add in your sources:
```
sources:
  - name: official
    remote: https://github.com/barbu-it/paasify-collection-official.git
```

Then you can reference any apps in your stacks:
```
stacks:
  - app: official:worpress
```

Then apply your changes with paasify:
```
$ paasify apply
```


## Project

### Requirements

The following requirements must be installed for this project:

* docker

To modify this project:

* paasify
* git

### Paasify documentation

Quicklinks:

* [Paasify Documentation](https://barbu-it.github.io/paasify/)
* [Paasify Sources](https://github.com/barbu-it/paasify)
* [Paasify Gitter](https://gitter.im/barbu-it/paasify)


## Project Informations

Paasify project maintened by:

* Author: mrjk
* License: GPLv3
* Repository: [github.com/barbu-it/paasify-collection-official](https://github.com/barbu-it/paasify-collection-official.git)

