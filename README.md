# transpopy
Read pot files to translate strings in msgid with google translate API and save a new po file.

[![Build Status](https://travis-ci.org/kanazux/transpopy.svg?branch=master)](https://travis-ci.org/kanazux/transpopy)

### Install

#### With PyPi
```console
kanazuchi@FreeBSD #: virtualenv --python=python3 .
kanazuchi@FreeBSD #: source bin/activate
kanazuchi@FreeBSD #: pip3 install transpopy
```

#### With BSD pkg
```console
kanazuchi@FreeBSD #: pkg install py36-transpopy
```

#### With GitHub
```console
kanazuchi@FreeBSD #: git clone https://github.com/kanazux/transpopy
kanazuchi@FreeBSD #: python3 setup.py install
```

### Usage:
> transpopy -f *samples/leap-seconds.pot* -o *newfile.po* -t *zh_cn* -e -i -p
![leap-seconds to chinese language](http://kanazuchi.com/static/chinese.jpg)

#### Help:
Translate msgid from po file with google translate API

```console
optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  Get the po file name to translated msgid's.
  -o OUTPUT_FILE, --output_file OUTPUT_FILE
                        Get a name to save new po file.
  -l LANG, --lang LANG  Get original language of po file.
  -t TRANSLATE, --translate TRANSLATE
                        Get language to translate the po file strings.
  -i, --imprecise       Write messages as fuzzy.
  -e, --error           Print some errors if exists.
  -p, --print_process   Print translate process.
```
