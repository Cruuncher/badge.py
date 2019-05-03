<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
-->

[![](https://img.shields.io/pypi/pyversions/badge.svg?longCache=True)](https://pypi.org/project/badge/)
[![](https://img.shields.io/pypi/v/badge.svg?maxAge=3600)](https://pypi.org/project/badge/)
[![Travis](https://api.travis-ci.org/looking-for-a-job/badge.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/badge.py/)

#### Installation
```bash
$ [sudo] pip install badge
```

#### Features
+   **md** (default), **rst**, **html**
+   autoformat strings
+   **minimalistic design**

#### Classes
class|`__doc__`
-|-
`badge.Badge` |badge generator class

#### Examples
```python
>>> class Travis(badge.Badge):
    title = "Travis"
    image = "https://api.travis-ci.org/{fullname}.svg?branch={branch}"
    link = "https://travis-ci.org/{fullname}/"

>>> Travis(fullname="owner/repo") # .md, Markdown by default
'[![Travis](https://api.travis-ci.org/owner/repo.svg?branch=master)](https://travis-ci.org/owner/repo/)'

>>> Travis(fullname="owner/repo").rst # .rst, reStructuredText
'.. image: : https://api.travis-ci.org/owner/repo.svg?branch=master
    : target: https://travis-ci.org/owner/repo/'
```

<p align="center">
    <a href="https://pypi.org/project/python-readme-generator/">python-readme-generator</a>
</p>