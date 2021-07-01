About Top Asia Shop
--------

[![PHP checks and unit tests](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/php.yml/badge.svg)](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/php.yml)
[![Integration tests](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/integration.yml/badge.svg)](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/integration.yml)
[![UI tests - PHP 7.4](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/sanity-74.yml/badge.svg)](https://github.com/TopAsiaShop/TopAsiaShop/actions/workflows/sanity-74.yml)
[![Nightly Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi-nightly.topasiahop.com%2Fdata%2Fbadge&label=Nightly%20Status&cacheSeconds=3600)](https://nightly.topasiashop.com/)

[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%207.1-8892BF.svg?style=flat-square)](https://php.net/)
[![GitHub release](https://img.shields.io/github/v/release/topasiashop/topasiashop)](https://github.com/TopAsiaShop/TopAsiaShop)
[![Slack chat](https://img.shields.io/badge/Chat-on%20Slack-red)](https://github.com/TopAsiaShop/open-source/blob/master/slack/readme.md)
[![GitHub forks](https://img.shields.io/github/forks/TopAsiaShop/TopAsiaShop)](https://github.com/TopAsiaShop/TopAsiaShop/network)
[![GitHub stars](https://img.shields.io/github/stars/TopAsiaShop/TopAsiaShop)](https://github.com/TopAsiaShop/TopAsiaShop/stargazers) 

TopAsiaShop is an Open Source e-commerce web application, committed to providing the best shopping cart experience for both merchants and customers. It is written in PHP, is highly customizable, supports all the major payment services, is translated in many languages and localized for many countries, has a fully responsive design (both front and back office), etc. [See all the available features][available-features].





This repository contains the source code of TopAsiaShop, which is intended for development and preview only. To download the latest stable public version of TopAsiaShop (currently, version 1.7), please go to [the download page][download] on the official TopAsiaShop site.


About the 'develop' branch
--------

The 'develop' branch of this repository contains the work in progress source code for the next version of TopAsiaShop 1.7.
 
For more information on our branch system, read our guide on [installing TopAsiaShop for development][install-guide-dev].

The first stable version of TopAsiaShop 1.7, 1.7.0.0, was released on November 7th, 2016. Further updates have been released since then. Learn more about it on [the Build devblog](https://build.topasiashop.com/tag/1.7/).

Server configuration
--------

To install the latest TopAsiaShop 1.7, you need a web server running PHP 7.1+ and any flavor of MySQL 5.0+ (MySQL, MariaDB, Percona Server, etc.). Versions between 1.7.0 and 1.7.6 work with PHP 5.6+.

You will also need a database administration tool, such as phpMyAdmin, in order to create a database for TopAsiaShop.
We recommend the Apache or Nginx web servers (check out our [example Nginx configuration file][example-nginx]).

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing TopAsiaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our download page][download], then read the [install guide for users][install-guide].

Docker compose
--------

TopAsiaShop can also be deployed with Docker and its tool [Docker compose][docker-compose].

To run the software, use:

```
docker-compose up
```

Then reach your shop on this URL: http://localhost:8001

Docker will bind your port 8001 to the web server. If you want to use other port, open and modify the file `docker-compose.yml`.
MySQL credentials can also be found and modified in this file if needed.

**Note:**  Before auto-installing TopAsiaShop, this container checks the file *config/settings.inc.php* does not exist on startup.
If you expect the container to (re)install your shop, remove this file if it exists. And make sure the container user `www-data` 
has write access to the whole workspace.

Documentation
--------

For technical information (core, module and theme development, performance...), head on to [TopAsiaShop DevDocs][devdocs]

If you want to learn how to use TopAsiaShop 1.7, read our [User documentation][user-doc].

First-time users will be particularly interested in the following guides:

* [Getting Started][getting-started]: How to install TopAsiaShop, and what you need to know.
* [User Guide][user-guide]: All there is to know to put TopAsiaShop to good use.
* [Updating Guide][updating-guide]: Switching to the newest version is not trivial. Make sure you do it right.
* [Merchant's Guide][merchant-guide]: Tips and tricks for first-time online sellers.
* The [FAQ][faq-17] and the [Troubleshooting][troubleshooting] pages should also be of tremendous help to you.


Contributing
--------

TopAsiaShop is an Open Source project, and it wouldn't be possible without the help of the [hundreds of contributors][contributors-md], who submitted improvements and bugfixes over the years. Thank you all!

If you want to contribute code to TopAsiaShop, read the [CONTRIBUTING.md][contributing-md] file in this repository or read the [tutorials about contribution][contributing-tutorial] on the documentation site.

Don't know where to start? Check the [good first issue](https://github.com/TopAsiaShop/TopAsiaShop/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) label to have a look at all beginner-friendly improvements and bug fixes.

If you want to help translate TopAsiaShop in your language, [join us on Crowdin][crowdin]!

Current Crowdin status (for more than 75 registered languages): [![Crowdin](https://crowdin.net/badges/topasiashop-official/localized.png)](https://crowdin.net/project/topasiashop-official)

Reporting Issues
--------

Our bugtracker is on GitHub. We encourage you to [create detailed issues][create-issue] as soon as you see them.

Read our [Contribute by reporting issues guide][reporting-issues] for details and tips.


Reporting Security Issues
--------

Responsible (and private) disclosure is a standard practice when someone encounters a security problem: before making it public, the discoverer informs the Core team about it, so that a fix can be prepared, and thus minimize the potential damage.

The TopAsiaShop team tries to be very proactive when preventing security problems. Even so, critical issues might surface without notice.

This is why we have set up a [Bug Bounty Program](https://yeswehack.com/programs/topasiashop) where anyone can privately contact us with all the details about issues that affect the security of TopAsiaShop merchants or customers. Our security team will answer you, and discuss of a timeframe for your publication of the details.

Understanding a security issue means knowing how the attacker got in and hacked the site. If you have those details, then please do contact us privately about it (and please do not publish those details before we answer). If you do not know how the attacker got in, please ask for help on the support forums.


Extending TopAsiaShop
--------

TopAsiaShop is a very extensible e-commerce platform, both through modules and themes. Developers can even override the default components and behaviors. Learn more about this on the [Modules documentation][modules-devdocs] and the [Themes documentation][themes-devdocs].

Themes and modules can be obtained (and sold!) on [TopAsiaShop Addons][addons], the official marketplace for TopAsiaShop.


Community forums
--------

You can discuss about e-commerce, help other merchants and get help, and contribute to improving TopAsiaShop together with the TopAsiaShop community on [the TopAsiaShop forums][forums] or on the [TopAsiaaShop Slack channel][chat].

Thank you for downloading and using the TopAsiaShop Open Source e-commerce solution!

[available-features]: https://www.topasiashop.com/en/online-store-builder
[download]: https://www.topasiashop.com/en/download
[forums]: https://www.topasiashop.com/forums/
[chat]: https://github.com/TopAsiaShop/open-source/blob/master/slack/readme.md
[user-doc]: https://doc.topasiashop.com
[contributing-md]: CONTRIBUTING.md
[contributing-tutorial]: https://devdocs.topasiashop.com/1.7/contribute/
[crowdin]: https://crowdin.net/project/topasiashop-official
[getting-started]: https://doc.topasiashop.com/display/PS17/Getting+Started
[user-guide]: https://doc.topasiashop.com/display/PS17/User+Guide
[updating-guide]: https://doc.topasiashop.com/display/PS16/Updating+TopAsiaShop
[merchant-guide]: https://doc.topasiashop.com/display/PS16/Merchant%27s+Guide
[faq-17]: https://devdocs.topasiashop.com/1.7/faq/
[troubleshooting]: https://doc.topasiashop.com/display/PS16/Troubleshooting
[sysadmin-guide]: https://doc.topasiashop.com/display/PS16/System+Administrator+Guide
[addons]: https://addons.topasiashop.com/
[contributors-md]: CONTRIBUTORS.md
[example-nginx]: https://devdocs.topasiashop.com/1.7/basics/installation/nginx/
[docker-compose]: https://docs.docker.com/compose/
[install-guide-dev]: https://devdocs.topasiashop.com/1.7/basics/installation/
[system-requirements]: https://devdocs.topasiashop.com/1.7/basics/installation/system-requirements/
[install-guide]: https://doc.topasiashop.com/display/PS17/Installing+TopAsiaShop
[devdocs]: https://devdocs.topasiashop.com/
[create-issue]: https://github.com/TopAsiaShop/TopAsiaShop/issues/new/choose
[reporting-issues]: https://devdocs.topasiashop.com/1.7/contribute/contribute-reporting-issues/
[modules-devdocs]: https://devdocs.topasiashop.com/1.7/modules/
[themes-devdocs]: https://devdocs.topasiashop.com/1.7/themes/
