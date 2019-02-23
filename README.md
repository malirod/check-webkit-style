# Webkit style checker

Separate [Webkit style](https://webkit.org/code-style-guidelines/) checker. Extracted from WebKit code base with removed dependencies.

Extracted from snapshot of the WebKit source tree taken from http://webkit.org/getting-the-code (19 Feb 2019)

Original location: `Tools/Scripts`

Known checkers:

- cpp
- cmake
- changelog
- javascipt
- json
- png
- python
- text
- xcodeproj
- xml

## Usage

Detailed help: `<tool-path>/check-webkit-style -h`

Sample usage: `<tool-path>/check-webkit-style check-webkit-style ./src ./test`

## Changed

- removed dependencies on WebKit scripts not related to style checking.
- tuned rule which required config.h to be the first header: requirement removed.

## Changed files

- `./webkitpy/port/__init__.py`
- `./webkitpy/style/main.py`
- `./webkitpy/style/checker.py`
- `./webkitpy/style/checkers/cpp.py`
