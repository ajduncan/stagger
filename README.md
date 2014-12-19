# Stagger #

Stagger is a BSD licensed ID3v1/ID3v2 tag manipulation package written in pure Python 3.

The ID3v2 tag format is notorious for its useless specification documents and its quirky, mutually incompatible part-implementations. Stagger is to provide a robust tagging package that is able to handle all the various badly formatted tags out there and allow you to convert them to a consensus format.

## Developing ##

Make sure you have python3 installed, create a virtual environment e.g.;

    $ virtualenv -p python3 .env
    $ source .env/bin/activate
    (.env) $ pip install -e .

## Features ##

* Reads and writes ID3 v1.0, 1.1, 2.2, 2.3 and 2.4 tags.
* Supports conversion between tag versions.
* Supports unsynchronized tags (all versions) and compressed frames (2.3 and 2.4 only).
* Full Unicode support, with customizable text encoding preferences.
* Has built-in support for all standard frame types (plus a few nonstandard ones). Easily extensible with additional frame types if needed.
* Supports duplicate frames and multiple text strings in a single frame.
* Supports reading/writing frames of unrecognized types and frames with invalid data. Automatically recognizes unknown text and URL frames.
* The order of frames in a tag is fully customizable.
* Package comes with extensive unit tests for an extra measure of code kwalitee.
* Tested under Mac OS X, Windows and GNU/Linux.