# api documentation for  [mobile-detect (v1.3.5)](http://hgoebl.github.io/mobile-detect.js/)  [![npm package](https://img.shields.io/npm/v/npmdoc-mobile-detect.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mobile-detect) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mobile-detect.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mobile-detect)
#### Device detection (phone, tablet, desktop, mobile grade, os, versions)

[![NPM](https://nodei.co/npm/mobile-detect.png?downloads=true)](https://www.npmjs.com/package/mobile-detect)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mobile-detect/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mobile-detect_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mobile-detect/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mobile-detect/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mobile-detect/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Heinrich Goebl",
        "email": "hgoebl@goebl.com",
        "url": "http://www.goebl.com/"
    },
    "bugs": {
        "url": "https://github.com/hgoebl/mobile-detect.js/issues"
    },
    "dependencies": {},
    "description": "Device detection (phone, tablet, desktop, mobile grade, os, versions)",
    "devDependencies": {
        "grunt": "~1.0.1",
        "grunt-contrib-concat": "~1.0.1",
        "grunt-contrib-copy": "~1.0.0",
        "grunt-contrib-jshint": "~1.0.0",
        "grunt-contrib-uglify": "~2.0.0",
        "grunt-contrib-watch": "~1.0.0",
        "grunt-exec": "~1.0.0",
        "grunt-jasmine-node": "~0.3.1",
        "grunt-jsdoc": "~2.1.0",
        "jshint": "2.9.2",
        "moment": "^2.14.1",
        "mote": "0.2.0",
        "uglify-js": "~2.7.0",
        "wordwrap": "1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "96d6511284f35d352eaf71baef459c61aebd30b2",
        "tarball": "https://registry.npmjs.org/mobile-detect/-/mobile-detect-1.3.5.tgz"
    },
    "gitHead": "a83eba55e21e3bf5dacef740964cd2ea27b4a5b3",
    "homepage": "http://hgoebl.github.io/mobile-detect.js/",
    "keywords": [
        "useragent",
        "mobile",
        "phone",
        "tablet",
        "detect",
        "device",
        "browser",
        "version",
        "mobilegrade",
        "sniff"
    ],
    "license": "MIT",
    "main": "mobile-detect.js",
    "maintainers": [
        {
            "name": "hgoebl",
            "email": "hgoebl@goebl.com"
        }
    ],
    "name": "mobile-detect",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/hgoebl/mobile-detect.js.git"
    },
    "scripts": {
        "test": "grunt jasmine_node"
    },
    "typings": "mobile-detect",
    "version": "1.3.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mobile-detect](#apidoc.module.mobile-detect)
1.  [function <span class="apidocSignatureSpan">mobile-detect.</span>isPhoneSized ()](#apidoc.element.mobile-detect.isPhoneSized)
1.  object <span class="apidocSignatureSpan">mobile-detect.</span>_impl
1.  string <span class="apidocSignatureSpan">mobile-detect.</span>version

#### [module mobile-detect._impl](#apidoc.module.mobile-detect._impl)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>detectOS (ua)](#apidoc.element.mobile-detect._impl.detectOS)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>findMatch (rules, userAgent)](#apidoc.element.mobile-detect._impl.findMatch)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>findMatches (rules, userAgent)](#apidoc.element.mobile-detect._impl.findMatches)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getDeviceSmallerSide ()](#apidoc.element.mobile-detect._impl.getDeviceSmallerSide)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getVersion (propertyName, userAgent)](#apidoc.element.mobile-detect._impl.getVersion)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getVersionStr (propertyName, userAgent)](#apidoc.element.mobile-detect._impl.getVersionStr)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>isMobileFallback (userAgent)](#apidoc.element.mobile-detect._impl.isMobileFallback)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>isTabletFallback (userAgent)](#apidoc.element.mobile-detect._impl.isTabletFallback)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>mobileGrade (t)](#apidoc.element.mobile-detect._impl.mobileGrade)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>prepareDetectionCache (cache, userAgent, maxPhoneWidth)](#apidoc.element.mobile-detect._impl.prepareDetectionCache)
1.  [function <span class="apidocSignatureSpan">mobile-detect._impl.</span>prepareVersionNo (version)](#apidoc.element.mobile-detect._impl.prepareVersionNo)
1.  object <span class="apidocSignatureSpan">mobile-detect._impl.</span>detectMobileBrowsers
1.  object <span class="apidocSignatureSpan">mobile-detect._impl.</span>mobileDetectRules
1.  string <span class="apidocSignatureSpan">mobile-detect._impl.</span>FALLBACK_MOBILE
1.  string <span class="apidocSignatureSpan">mobile-detect._impl.</span>FALLBACK_PHONE
1.  string <span class="apidocSignatureSpan">mobile-detect._impl.</span>FALLBACK_TABLET



# <a name="apidoc.module.mobile-detect"></a>[module mobile-detect](#apidoc.module.mobile-detect)

#### <a name="apidoc.element.mobile-detect.isPhoneSized"></a>[function <span class="apidocSignatureSpan">mobile-detect.</span>isPhoneSized ()](#apidoc.element.mobile-detect.isPhoneSized)
- description and source-code
```javascript
isPhoneSized = function () {}
```
- example usage
```shell
...
    cache.mobile = cache.phone = phone;
    cache.tablet = null;
    return; // unambiguously identified as phone
}

// our rules haven't found a match -> try more general fallback rules
if (impl.isMobileFallback(userAgent)) {
    phoneSized = MobileDetect.isPhoneSized(maxPhoneWidth);
    if (phoneSized === undefined) {
        cache.mobile = impl.FALLBACK_MOBILE;
        cache.tablet = cache.phone = null;
    } else if (phoneSized) {
        cache.mobile = cache.phone = impl.FALLBACK_PHONE;
        cache.tablet = null;
    } else {
...
```



# <a name="apidoc.module.mobile-detect._impl"></a>[module mobile-detect._impl](#apidoc.module.mobile-detect._impl)

#### <a name="apidoc.element.mobile-detect._impl.detectOS"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>detectOS (ua)](#apidoc.element.mobile-detect._impl.detectOS)
- description and source-code
```javascript
detectOS = function (ua) {
    return impl.findMatch(impl.mobileDetectRules.oss0, ua) ||
        impl.findMatch(impl.mobileDetectRules.oss, ua);
}
```
- example usage
```shell
...
 * iOS, MeeGoOS, MaemoOS, JavaOS, webOS, badaOS, BREWOS</tt><br>
 *
 * @returns {String} the key for the detected operating system.
 * @function MobileDetect#os
 */
os: function () {
    if (this._cache.os === undefined) {
        this._cache.os = impl.detectOS(this.ua);
    }
    return this._cache.os;
},

/**
 * Get the version (as Number) of the given property in the User-Agent.
 * <br>
...
```

#### <a name="apidoc.element.mobile-detect._impl.findMatch"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>findMatch (rules, userAgent)](#apidoc.element.mobile-detect._impl.findMatch)
- description and source-code
```javascript
findMatch = function (rules, userAgent) {
    for (var key in rules) {
        if (hasOwnProp.call(rules, key)) {
            if (rules[key].test(userAgent)) {
                return key;
            }
        }
    }
    return null;
}
```
- example usage
```shell
...
    impl.prepareDetectionCache = function (cache, userAgent, maxPhoneWidth) {
if (cache.mobile !== undefined) {
    return;
}
var phone, tablet, phoneSized;

// first check for stronger tablet rules, then phone (see issue#5)
tablet = impl.findMatch(impl.mobileDetectRules.tablets, userAgent);
if (tablet) {
    cache.mobile = cache.tablet = tablet;
    cache.phone = null;
    return; // unambiguously identified as tablet
}

phone = impl.findMatch(impl.mobileDetectRules.phones, userAgent);
...
```

#### <a name="apidoc.element.mobile-detect._impl.findMatches"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>findMatches (rules, userAgent)](#apidoc.element.mobile-detect._impl.findMatches)
- description and source-code
```javascript
findMatches = function (rules, userAgent) {
    var result = [];
    for (var key in rules) {
        if (hasOwnProp.call(rules, key)) {
            if (rules[key].test(userAgent)) {
                result.push(key);
            }
        }
    }
    return result;
}
```
- example usage
```shell
...
 * providing one of the defined keys as first argument to {@link MobileDetect#is}.
 *
 * @returns {Array} the array of detected user-agent keys or <tt>[]</tt>
 * @function MobileDetect#userAgents
 */
userAgents: function () {
    if (this._cache.userAgents === undefined) {
        this._cache.userAgents = impl.findMatches(impl.mobileDetectRules.uas, this.ua);
    }
    return this._cache.userAgents;
},

/**
 * Returns the detected operating system string or <tt>null</tt>.
 * <br>
...
```

#### <a name="apidoc.element.mobile-detect._impl.getDeviceSmallerSide"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getDeviceSmallerSide ()](#apidoc.element.mobile-detect._impl.getDeviceSmallerSide)
- description and source-code
```javascript
getDeviceSmallerSide = function () {
    return window.screen.width < window.screen.height ?
        window.screen.width :
        window.screen.height;
}
```
- example usage
```shell
...
        return this._cache.grade;
    }
};

// environment-dependent
if (typeof window !== 'undefined' && window.screen) {
    MobileDetect.isPhoneSized = function (maxPhoneWidth) {
        return maxPhoneWidth < 0 ? undefined : impl.getDeviceSmallerSide() <= maxPhoneWidth;
    };
} else {
    MobileDetect.isPhoneSized = function () {};
}

// should not be replaced by a completely new object - just overwrite existing methods
MobileDetect._impl = impl;
...
```

#### <a name="apidoc.element.mobile-detect._impl.getVersion"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getVersion (propertyName, userAgent)](#apidoc.element.mobile-detect._impl.getVersion)
- description and source-code
```javascript
getVersion = function (propertyName, userAgent) {
    var version = impl.getVersionStr(propertyName, userAgent);
    return version ? impl.prepareVersionNo(version) : NaN;
}
```
- example usage
```shell
...
 * Phone, Windows CE, Windows NT, Symbian, webOS</tt><br>
 *
 * @returns {Number} the version as float or <tt>NaN</tt> if User-Agent doesn't contain this version.
 *          Be careful when comparing this value with '==' operator!
 * @function MobileDetect#version
 */
version: function (key) {
    return impl.getVersion(key, this.ua);
},

/**
 * Get the version (as String) of the given property in the User-Agent.
 * <br>
 *
 * @param {String} key a key defining a thing which has a version.<br>
...
```

#### <a name="apidoc.element.mobile-detect._impl.getVersionStr"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>getVersionStr (propertyName, userAgent)](#apidoc.element.mobile-detect._impl.getVersionStr)
- description and source-code
```javascript
getVersionStr = function (propertyName, userAgent) {
    var props = impl.mobileDetectRules.props, patterns, i, len, match;
    if (hasOwnProp.call(props, propertyName)) {
        patterns = props[propertyName];
        len = patterns.length;
        for (i = 0; i < len; ++i) {
            match = patterns[i].exec(userAgent);
            if (match !== null) {
                return match[1];
            }
        }
    }
    return null;
}
```
- example usage
```shell
...
 *
 * @param {String} propertyName
 * @param {String} userAgent
 * @return {Number} version or <tt>NaN</tt> if version not found
 * @private
 */
impl.getVersion = function (propertyName, userAgent) {
    var version = impl.getVersionStr(propertyName, userAgent);
    return version ? impl.prepareVersionNo(version) : NaN;
};

/**
 * Prepare the version number.
 *
 * @param {String} version
...
```

#### <a name="apidoc.element.mobile-detect._impl.isMobileFallback"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>isMobileFallback (userAgent)](#apidoc.element.mobile-detect._impl.isMobileFallback)
- description and source-code
```javascript
isMobileFallback = function (userAgent) {
    return impl.detectMobileBrowsers.fullPattern.test(userAgent) ||
        impl.detectMobileBrowsers.shortPattern.test(userAgent.substr(0,4));
}
```
- example usage
```shell
...
if (phone) {
    cache.mobile = cache.phone = phone;
    cache.tablet = null;
    return; // unambiguously identified as phone
}

// our rules haven't found a match -> try more general fallback rules
if (impl.isMobileFallback(userAgent)) {
    phoneSized = MobileDetect.isPhoneSized(maxPhoneWidth);
    if (phoneSized === undefined) {
        cache.mobile = impl.FALLBACK_MOBILE;
        cache.tablet = cache.phone = null;
    } else if (phoneSized) {
        cache.mobile = cache.phone = impl.FALLBACK_PHONE;
        cache.tablet = null;
...
```

#### <a name="apidoc.element.mobile-detect._impl.isTabletFallback"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>isTabletFallback (userAgent)](#apidoc.element.mobile-detect._impl.isTabletFallback)
- description and source-code
```javascript
isTabletFallback = function (userAgent) {
    return impl.detectMobileBrowsers.tabletPattern.test(userAgent);
}
```
- example usage
```shell
...
        } else if (phoneSized) {
            cache.mobile = cache.phone = impl.FALLBACK_PHONE;
            cache.tablet = null;
        } else {
            cache.mobile = cache.tablet = impl.FALLBACK_TABLET;
            cache.phone = null;
        }
    } else if (impl.isTabletFallback(userAgent)) {
        cache.mobile = cache.tablet = impl.FALLBACK_TABLET;
        cache.phone = null;
    } else {
        // not mobile at all!
        cache.mobile = cache.tablet = cache.phone = null;
    }
};
...
```

#### <a name="apidoc.element.mobile-detect._impl.mobileGrade"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>mobileGrade (t)](#apidoc.element.mobile-detect._impl.mobileGrade)
- description and source-code
```javascript
mobileGrade = function (t) {
    // impl note:
    // To keep in sync w/ Mobile_Detect.php easily, the following code is tightly aligned to the PHP version.
    // When changes are made in Mobile_Detect.php, copy this method and replace:
    //     $this-> / t.
    //     self::MOBILE_GRADE_(.) / '$1'
    //     , self::VERSION_TYPE_FLOAT / (nothing)
    //     isIOS() / os('iOS')
    //     [reg] / (nothing)   <-- jsdelivr complaining about unescaped unicode character U+00AE
    var $isMobile = t.mobile() !== null;

    if (
        // Apple iOS 3.2-5.1 - Tested on the original iPad (4.3 / 5.0), iPad 2 (4.3), iPad 3 (5.1), original iPhone (3.1), iPhone
 3 (3.2), 3GS (4.3), 4 (4.3 / 5.0), and 4S (5.1)
        t.os('iOS') && t.version('iPad')>=4.3 ||
        t.os('iOS') && t.version('iPhone')>=3.1 ||
        t.os('iOS') && t.version('iPod')>=3.1 ||

        // Android 2.1-2.3 - Tested on the HTC Incredible (2.2), original Droid (2.2), HTC Aria (2.1), Google Nexus S (2.3). Functional
 on 1.5 & 1.6 but performance may be sluggish, tested on Google G1 (1.5)
        // Android 3.1 (Honeycomb)  - Tested on the Samsung Galaxy Tab 10.1 and Motorola XOOM
        // Android 4.0 (ICS)  - Tested on a Galaxy Nexus. Note: transition performance can be poor on upgraded devices
        // Android 4.1 (Jelly Bean)  - Tested on a Galaxy Nexus and Galaxy 7
        ( t.version('Android')>2.1 && t.is('Webkit') ) ||

        // Windows Phone 7-7.5 - Tested on the HTC Surround (7.0) HTC Trophy (7.5), LG-E900 (7.5), Nokia Lumia 800
        t.version('Windows Phone OS')>=7.0 ||

        // Blackberry 7 - Tested on BlackBerry Torch 9810
        // Blackberry 6.0 - Tested on the Torch 9800 and Style 9670
        t.is('BlackBerry') && t.version('BlackBerry')>=6.0 ||
        // Blackberry Playbook (1.0-2.0) - Tested on PlayBook
        t.match('Playbook.*Tablet') ||

        // Palm WebOS (1.4-2.0) - Tested on the Palm Pixi (1.4), Pre (1.4), Pre 2 (2.0)
        ( t.version('webOS')>=1.4 && t.match('Palm|Pre|Pixi') ) ||
        // Palm WebOS 3.0  - Tested on HP TouchPad
        t.match('hp.*TouchPad') ||

        // Firefox Mobile (12 Beta) - Tested on Android 2.3 device
        ( t.is('Firefox') && t.version('Firefox')>=12 ) ||

        // Chrome for Android - Tested on Android 4.0, 4.1 device
        ( t.is('Chrome') && t.is('AndroidOS') && t.version('Android')>=4.0 ) ||

        // Skyfire 4.1 - Tested on Android 2.3 device
        ( t.is('Skyfire') && t.version('Skyfire')>=4.1 && t.is('AndroidOS') && t.version('Android')>=2.3 ) ||

        // Opera Mobile 11.5-12: Tested on Android 2.3
        ( t.is('Opera') && t.version('Opera Mobi')>11 && t.is('AndroidOS') ) ||

        // Meego 1.2 - Tested on Nokia 950 and N9
        t.is('MeeGoOS') ||

        // Tizen (pre-release) - Tested on early hardware
        t.is('Tizen') ||

        // Samsung Bada 2.0 - Tested on a Samsung Wave 3, Dolphin browser
        // @todo: more tests here!
        t.is('Dolfin') && t.version('Bada')>=2.0 ||

        // UC Browser - Tested on Android 2.3 device
        ( (t.is('UC Browser') || t.is('Dolfin')) && t.version('Android')>=2.3 ) ||

        // Kindle 3 and Fire  - Tested on the built-in WebKit browser for each
        ( t.match('Kindle Fire') ||
            t.is('Kindle') && t.version('Kindle')>=3.0 ) ||

        // Nook Color 1.4.1 - Tested on original Nook Color, not Nook Tablet
        t.is('AndroidOS') && t.is('NookTablet') ||

        // Chrome Desktop 11-21 - Tested on OS X 10.7 and Windows 7
        t.version('Chrome')>=11 && !$isMobile ||

        // Safari Desktop 4-5 - Tested on OS X 10.7 and Windows 7
        t.version('Safari')>=5.0 && !$isMobile ||

        // Firefox Desktop 4-13 - Tested on OS X 10.7 and Windows 7
        t.version('Firefox')>=4.0 && !$isMobile ||

        // Internet Explorer 7-9 - Tested on Windows XP, Vista and 7
        t.version('MSIE')>=7.0 && !$isMobile ||

        // Opera Desktop 10-12 - Tested on OS X 10.7 and Windows 7
        // @reference: http://my.opera.com/community/openweb/idopera/
        t.version('Opera')>=10 && !$isMobile ...
```
- example usage
```shell
...
*     <strong>Find information how to download and install:</strong>
*     <a href="https://github.com/hgoebl/mobile-detect.js/">github.com/hgoebl/mobile-detect.js/</a>
* </div>
*
* @example <pre>
*     var md = new MobileDetect(window.navigator.userAgent);
*     if (md.mobile()) {
*         location.href = (md.mobileGrade() === 'A') ? '/mobile/' : '/lynx/';
*     }
* </pre>
*
* @param {string} userAgent typically taken from window.navigator.userAgent or http_header['User-Agent']
* @param {number} [maxPhoneWidth=600] <strong>only for browsers</strong> specify a value for the maximum
*        width of smallest device side (in logical "CSS" pixels) until a device detected as mobile will be handled
*        as phone.
...
```

#### <a name="apidoc.element.mobile-detect._impl.prepareDetectionCache"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>prepareDetectionCache (cache, userAgent, maxPhoneWidth)](#apidoc.element.mobile-detect._impl.prepareDetectionCache)
- description and source-code
```javascript
prepareDetectionCache = function (cache, userAgent, maxPhoneWidth) {
    if (cache.mobile !== undefined) {
        return;
    }
    var phone, tablet, phoneSized;

    // first check for stronger tablet rules, then phone (see issue#5)
    tablet = impl.findMatch(impl.mobileDetectRules.tablets, userAgent);
    if (tablet) {
        cache.mobile = cache.tablet = tablet;
        cache.phone = null;
        return; // unambiguously identified as tablet
    }

    phone = impl.findMatch(impl.mobileDetectRules.phones, userAgent);
    if (phone) {
        cache.mobile = cache.phone = phone;
        cache.tablet = null;
        return; // unambiguously identified as phone
    }

    // our rules haven't found a match -> try more general fallback rules
    if (impl.isMobileFallback(userAgent)) {
        phoneSized = MobileDetect.isPhoneSized(maxPhoneWidth);
        if (phoneSized === undefined) {
            cache.mobile = impl.FALLBACK_MOBILE;
            cache.tablet = cache.phone = null;
        } else if (phoneSized) {
            cache.mobile = cache.phone = impl.FALLBACK_PHONE;
            cache.tablet = null;
        } else {
            cache.mobile = cache.tablet = impl.FALLBACK_TABLET;
            cache.phone = null;
        }
    } else if (impl.isTabletFallback(userAgent)) {
        cache.mobile = cache.tablet = impl.FALLBACK_TABLET;
        cache.phone = null;
    } else {
        // not mobile at all!
        cache.mobile = cache.tablet = cache.phone = null;
    }
}
```
- example usage
```shell
...
 * <br>
 * In most cases you will use the return value just as a boolean.
 *
 * @returns {String} the key for the phone family or tablet family, e.g. "Nexus".
 * @function MobileDetect#mobile
 */
mobile: function () {
    impl.prepareDetectionCache(this._cache, this.ua, this.maxPhoneWidth);
    return this._cache.mobile;
},

/**
 * Returns the detected phone type/family string or <tt>null</tt>.
 * <br>
 * The returned tablet (family or producer) is one of following keys:<br>
...
```

#### <a name="apidoc.element.mobile-detect._impl.prepareVersionNo"></a>[function <span class="apidocSignatureSpan">mobile-detect._impl.</span>prepareVersionNo (version)](#apidoc.element.mobile-detect._impl.prepareVersionNo)
- description and source-code
```javascript
prepareVersionNo = function (version) {
    var numbers;

    numbers = version.split(/[a-z._ \/\-]/i);
    if (numbers.length === 1) {
        version = numbers[0];
    }
    if (numbers.length > 1) {
        version = numbers[0] + '.';
        numbers.shift();
        version += numbers.join('');
    }
    return Number(version);
}
```
- example usage
```shell
...
 * @param {String} propertyName
 * @param {String} userAgent
 * @return {Number} version or <tt>NaN</tt> if version not found
 * @private
 */
impl.getVersion = function (propertyName, userAgent) {
    var version = impl.getVersionStr(propertyName, userAgent);
    return version ? impl.prepareVersionNo(version) : NaN;
};

/**
 * Prepare the version number.
 *
 * @param {String} version
 * @return {Number} the version number as a floating number
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
