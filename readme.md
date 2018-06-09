# Shamir32

A tool using Shamir's Secret Sharing Scheme to split BIP32 HD wallets into fragments and recombine them for recovering addressess and private keys.

## Standalone offline version

Download `shamir32-standalone.html`

Open the file in a browser by double clicking it.

This can be compiled from source using the command `python compile.py`

# Tests

Tests depend on

* nodejs
* selenium webdriver - cd /path/to/shamir32/tests; npm install
* selenium driver for firefox ([geckodriver](https://github.com/mozilla/geckodriver/releases)) and / or chrome ([chromedriver](https://sites.google.com/a/chromium.org/chromedriver/downloads))
* jasmine - npm install --global jasmine

Before running tests, the site must be served at http://localhost:8000.

```
$ cd /path/to/shamir32/src
$ python -m http.server
```

Run tests from the command-line

```
$ cd /path/to/shamir32/tests
$ jasmine spec/tests.js
```

# License

This Shamir32 tool is released under the terms of the MIT license. See LICENSE for
more information or see https://opensource.org/licenses/MIT.
