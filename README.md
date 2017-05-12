# German Translations for Magento 2
> This Language Pack is forked from [splendidinternet/Magento2_German_LocalePack_de_DE](https://github.com/splendidinternet/Magento2_German_LocalePack_de_DE), and extended as needed for our usage.

You can read all about using this package in German over at [splendidinternet/Magento2_German_LocalePack_de_DE](https://github.com/splendidinternet/Magento2_German_LocalePack_de_DE).

Originally translated by native speakers this language pack is a full translation of Magento 2 - Front & Back. To provide an easy way to meet our ("Synoa GmbH") needs for additional translations and to provide a consistend location for the translations the original project was forked.

## Installation

### Manual Installation
Copy all files to `/app/i18n/synoa/de_DE/`. Then go into the Magento root directory, e.g. `/var/www/` and remove the pre-existing `js-translation.json` file, then deploy the static content for the `de_DE` language, run the upgrade command, remove `var/di` directory and finally regenerate it by running `bin/magento setup:di:deploy`.

```bash
rm pub/static/frontend/Magento/{theme}/de_DE/js-translation.json
php bin/magento setup:static-content:deploy de_DE
php bin/magento setup:upgrade
rm -rf var/di
php bin/magento setup:di:compile
```
_Note: replace {theme} with the theme currenlty in usage_

### Installation with Composer

```bash
composer require synoa/mage2-locale-de-de
rm pub/static/frontend/Magento/{theme}/de_DE/js-translation.json
php bin/magento setup:static-content:deploy de_DE
```
_Note: replace {theme} with the theme currenlty in usage_


---

## Credit

This repository is a fork of [splendidinternet/Magento2_German_LocalePack_de_DE](https://github.com/splendidinternet/Magento2_German_LocalePack_de_DE). The majority of translation work was done by [splendidinternet](https://github.com/splendidinternet/) as well as [a bunch of contributors](https://github.com/splendidinternet/Magento2_German_LocalePack_de_DE/graphs/contributors).

In compliance with the original license ([See LICENSE.txt](https://github.com/splendidinternet/Magento2_German_LocalePack_de_DE/blob/master/LICENSE.txt)) this modified version is distributed under the same Open Source License (Open Software License ("OSL") v. 3.0). You are free to fork, redistribute and build upon the work done by Synoa GmbH, however there is no warranty whatsoever. See [LICENSE.txt](https://github.com/synoa/Magento2_German_LocalePack_de_DE/blob/master/LICENSE.txt).
