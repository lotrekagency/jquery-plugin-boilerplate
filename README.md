# jQueryPluginBP

[![Build Status][travis-image]][travis-url] [![Coveralls Status][coveralls-image]][coveralls-url]
[![Latest Version](https://img.shields.io/pypi/v/jquerypluginbp.svg)](https://pypi.python.org/pypi/jquerypluginbp/)
[![Supported Python versions](https://img.shields.io/badge/python-2.7%2C%202.8%2C%203.3%2C%203.4-blue.svg)](https://pypi.python.org/pypi/jquerypluginbp/)
[![Downloads](https://img.shields.io/pypi/dm/jquerypluginbp.svg)](https://pypi.python.org/pypi/jquerypluginbp/)

A tool for generating jQuery plugins boilerplate code

## Install

    $ pip install jquerypluginbp

## Usage

Define your plugin.json manifest file

    $ jquerypluginbp yourmanifest.plugin.json

You can specify the destination path

    $ jquerypluginbp yourmanifest.plugin.json -d destination_path

## Manifest file example

    {
        "name": "gmap",
        "title": "jQuery Gmap Plugin",
        "description": "Convenient jQuery wrapper around Google Maps JavaScript API v3.",
        "keywords": [
            "google",
            "maps",
            "v3"
        ],
        "version": "0.1.0dev",
        "author": {
            "name": "Nephila"
        },
        "maintainers": [
            {
                "name": "Andrea Stagi",
                "email": "stagi.andrea@gmail.com",
                "url": "http://github.com/astagi"
            }
        ],
        "licenses": [
            {
                "type": "MIT",
                "url": ""
            }
        ],
        "dependencies": {
            "jquery": ">=1.4.4"
        }
    }

## Run tests

    $  nosetests --with-coverage --cover-package=jquerypluginbp.core

[travis-url]: https://travis-ci.org/nephila/jquerypluginbp
[travis-image]: http://img.shields.io/travis/nephila/jquerypluginbp.svg

[coveralls-url]: https://coveralls.io/r/nephila/jquerypluginbp
[coveralls-image]: http://img.shields.io/coveralls/nephila/jquerypluginbp/master.svg
