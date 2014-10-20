Uberpay Project
================

## Pré-requis

* Virtual box
* Vagrant

## Installation

* Télécharger de la VM `precise64` [Ubuntu 12.04.1 LTS x86_64 (Guest Additions 4.1.18)] : `vagrant box add precise64 http://files.vagrantup.com/precise64.box`
* Clone du repo `git clone https://github.com/ndussart/Uberpay.git`
* Initialisation des submodules `git submodule update --init`
* `mkdir puppet/modules/maven/files`
* Télécharger `apache-maven-3.1.1-bin.tar.gz` depuis [http://maven.apache.org](http://maven.apache.org) dans le répertoire `puppet/modules/maven/files`
* Terminer; `vagrant up`

## Utilisation

Le répertoire `webapp` est synchro avec `/vagrant`

Les ports 8080 et 5432 sont mappé sur leurs ports respectifs de la VM.

Pour se logguer sur la VM : `vagrant ssh`.

Postgres config : `puppet/manifests/base.pp`.


## Modules Installés

* [Java](https://github.com/puppetlabs/puppetlabs-java)
* [Postgresql](https://github.com/puppetlabs/puppet-postgresql)
* [Maven](https://github.com/7terminals/puppet-maven)

(dépendances non listées)

## Changelog

#### 20-10-2014

v0.000
