# crlang/browser.php

[![Build Status](https://travis-ci.org/crlang/Browser.php.png?branch=master)](https://travis-ci.org/crlang/Browser.php)

根据 User Agent 内容来通过PHP去检测用户的浏览器和平台信息

## 安装

可以下载到本地使用，或者通过 composer 安装依赖于所在的项目 [Composer](https://getcomposer.org/):
```
    composer require crlang/browser.php
```
如果只需要在开发期间用到此库，例如要运行项目的测试套件，建议应该将其添加为Dev依赖：
```
    composer require --dev crlang/browser.php
```

## 用法:

```php
$browser = new Browser();
echo $browser->getBrowser();
```

## 浏览器检测

该解决方案标识以下浏览器：

* Opera (`Browser::BROWSER_OPERA`)
* WebTV (`Browser::BROWSER_WEBTV`)
* NetPositive (`Browser::BROWSER_NETPOSITIVE`)
* Edge (`Browser::BROWSER_EDGE`)
* Internet Explorer (`Browser::BROWSER_IE`)
* Pocket Internet Explorer (`Browser::BROWSER_POCKET_IE`)
* Galeon (`Browser::BROWSER_GALEON`)
* Konqueror (`Browser::BROWSER_KONQUEROR`)
* iCab (`Browser::BROWSER_ICAB`)
* OmniWeb (`Browser::BROWSER_OMNIWEB`)
* Phoenix (`Browser::BROWSER_PHOENIX`)
* Firebird (`Browser::BROWSER_FIREBIRD`)
* UCBrowser (`Browser::BROWSER_UCBROWSER`)
* Firefox (`Browser::BROWSER_FIREFOX`)
* Mozilla (`Browser::BROWSER_MOZILLA`)
* Palemoon (`Browser::BROWSER_PALEMOON`)
* curl (`Browser::BROWSER_CURL`)
* wget (`Browser::BROWSER_WGET`)
* Amaya (`Browser::BROWSER_AMAYA`)
* Lynx (`Browser::BROWSER_LYNX`)
* Safari (`Browser::BROWSER_SAFARI`)
* Playstation (`Browser::BROWSER_PLAYSTATION`)
* iPhone (`Browser::BROWSER_IPHONE`)
* iPod (`Browser::BROWSER_IPOD`)
* Google.s Android(`Browser::BROWSER_ANDROID`)
* Google.s Chrome(`Browser::BROWSER_CHROME`)
* GoogleBot(`Browser::BROWSER_GOOGLEBOT`)
* Yahoo!.s Slurp(`Browser::BROWSER_SLURP`)
* W3C.s Validator(`Browser::BROWSER_W3CVALIDATOR`)
* BlackBerry(`Browser::BROWSER_BLACKBERRY`)

## 操作系统检测

该解决方案标识以下操作系统：

* Windows (`Browser::PLATFORM_WINDOWS`)
* Windows CE (`Browser::PLATFORM_WINDOWS_CE`)
* Apple (`Browser::PLATFORM_APPLE`)
* Linux (`Browser::PLATFORM_LINUX`)
* Android (`Browser::PLATFORM_ANDROID`)
* OS/2 (`Browser::PLATFORM_OS2`)
* BeOS (`Browser::PLATFORM_BEOS`)
* iPhone (`Browser::PLATFORM_IPHONE`)
* iPod (`Browser::PLATFORM_IPOD`)
* BlackBerry (`Browser::PLATFORM_BLACKBERRY`)
* FreeBSD (`Browser::PLATFORM_FREEBSD`)
* OpenBSD (`Browser::PLATFORM_OPENBSD`)
* NetBSD (`Browser::PLATFORM_NETBSD`)
* SunOS (`Browser::PLATFORM_SUNOS`)
* OpenSolaris (`Browser::PLATFORM_OPENSOLARIS`)
* iPad (`Browser::PLATFORM_IPAD`)

## 测试

使用 PHPUnit 对 tests/lists 中可用的已知用户代理进行测试。每个文件都是选项卡，其中包含以下字段：

用户代理，用户代理类型，浏览器，版本，操作系统，操作系统版本

例如
```
Opera/9.80 (X11; Linux i686; Ubuntu/14.10) Presto/2.12.388 Version/12.16	Browser	Opera	12.16	Linux	Linux
Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_2) AppleWebKit/535.1 (KHTML, like Gecko) Chrome/14.0.835.186 Safari/535.1   Browser	Chrome	14.0.835.186	Macintosh	OS X		10_7_2
```

测试可以运行 phpunit:

```bash
vendor/phpunit/phpunit/phpunit
```


