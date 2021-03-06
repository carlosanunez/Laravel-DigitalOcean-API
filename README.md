Laravel DigitalOcean API
======================


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/GrahamCampbell/Laravel-DigitalOcean-API/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
[![Build Status](https://travis-ci.org/GrahamCampbell/Laravel-DigitalOcean-API.png?branch=master)](https://travis-ci.org/GrahamCampbell/Laravel-DigitalOcean-API)
[![Latest Version](https://poser.pugx.org/graham-campbell/digitalocean-api/v/stable.png)](https://packagist.org/packages/graham-campbell/digitalocean-api)
[![Total Downloads](https://poser.pugx.org/graham-campbell/digitalocean-api/downloads.png)](https://packagist.org/packages/graham-campbell/digitalocean-api)
[![Scrutinizer Quality Score](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-DigitalOcean-API/badges/quality-score.png?s=b9089823ad760c37162693975409ce4415758b23)](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-DigitalOcean-API)
[![Still Maintained](http://stillmaintained.com/GrahamCampbell/Laravel-DigitalOcean-API.png)](http://stillmaintained.com/GrahamCampbell/Laravel-DigitalOcean-API)


## THIS ALPHA RELEASE IS FOR TESTING ONLY


## What Is Laravel DigitalOcean API?

Laravel DigitalOcean API is a [DigitalOcean API](https://api.digitalocean.com) client for [Laravel 4](http://laravel.com).  

* Laravel DigitalOcean API was created by, and is maintained by [Graham Campbell](https://github.com/GrahamCampbell).  
* Laravel DigitalOcean API relies on my [Core API](https://github.com/GrahamCampbell/Laravel-Core-API) package.  
* Laravel DigitalOcean API uses [Travis CI](https://travis-ci.org/GrahamCampbell/Laravel-DigitalOcean-API) to run tests to check if it's working as it should.  
* Laravel DigitalOcean API uses [Scrutinizer CI](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-DigitalOcean-API) to run additional tests and checks.  
* Laravel DigitalOcean API uses [Composer](https://getcomposer.org) to load and manage dependencies.  
* Laravel DigitalOcean API was not designed for user login, but for server use only.  
* Laravel DigitalOcean API provides a [change log](https://github.com/GrahamCampbell/Laravel-DigitalOcean-API/blob/master/CHANGELOG.md), [releases](https://github.com/GrahamCampbell/Laravel-DigitalOcean-API/releases), and a [wiki](https://github.com/GrahamCampbell/Laravel-DigitalOcean-API/wiki).  
* Laravel DigitalOcean API is licensed under the Apache License, available [here](https://github.com/GrahamCampbell/Laravel-DigitalOcean-API/blob/master/LICENSE.md).  


## System Requirements

* PHP 5.3.3+, 5.4+ or PHP 5.5+ is required.
* You will need [Laravel 4](http://laravel.com) because this package is designed for it.  
* You will need [Composer](https://getcomposer.org) installed to load the dependencies of Laravel CloudFlare-API.  


## Installation

Please check the system requirements before installing Laravel DigitalOcean API.  

To get the latest version of Laravel DigitalOcean API, simply require it in your `composer.json` file.

`"graham-campbell/digitalocean-api": "dev-master"`

You'll then need to run `composer install` or `composer update` to download it and have the autoloader updated.

Once Laravel DigitalOcean API is installed, you need to register the service provider. Open up `app/config/app.php` and add the following to the `providers` key.

`'GrahamCampbell\DigitalOceanAPI\DigitalOceanAPIServiceProvider'`

You will also need to have registered the [Laravel Core API](https://github.com/GrahamCampbell/Laravel-Core-API) service provider.

`'GrahamCampbell\CoreAPI\CoreAPIServiceProvider'`

You can register the DigitalOceanAPI facade in the `aliases` key of your `app/config/app.php` file if you like.

`'DigitalOceanAPI' => 'GrahamCampbell\DigitalOceanAPI\Facades\DigitalOceanAPI'`


## Updating Your Fork

The latest and greatest source can be found on [GitHub](https://github.com/GrahamCampbell/Laravel-DigitalOcean-API).  
Before submitting a pull request, you should ensure that your fork is up to date.  

You may fork Laravel DigitalOcean API:  

    git remote add upstream git://github.com/GrahamCampbell/Laravel-DigitalOcean-API.git

The first command is only necessary the first time. If you have issues merging, you will need to get a merge tool such as [P4Merge](http://perforce.com/product/components/perforce_visual_merge_and_diff_tools).  

You can then update the branch:  

    git pull --rebase upstream develop
    git push --force origin <branch_name>

Once it is set up, run `git mergetool`. Once all conflicts are fixed, run `git rebase --continue`, and `git push --force origin <branch_name>`.  


## Pull Requests

Please submit pull requests against the develop branch.  

* Any pull requests made against the master branch will be closed immediately.  
* If you plan to fix a bug, please create a branch called `fix-`, followed by an appropriate name.  
* If you plan to add a feature, please create a branch called `feature-`, followed by an appropriate name.  
* Please indent with 4 spaces rather than tabs, and make sure your code is commented.  


## License

Apache License  

Copyright 2013 Graham Campbell  

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at  

 http://www.apache.org/licenses/LICENSE-2.0  

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.  
