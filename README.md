puppet-svn-hooks
================

Subversion hook scripts to deal with a repository of puppet code.

License: MIT
------------
Copyright (c) 2012 Jason Hancock <jsnbyh@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is furnished
to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

Requirements
------------
  * `puppet >= 2.7` is installed on system
  * `puppet-lint` ruby gem is installed on system
  * `subversion` package is installed on system
  * Adjust `LINTFLAGS` variable as appropriate

HOOKS:
-------
**pre-commit:**

This pre-commit hook verifies that puppet can parse \*.pp files, that templates
(\*.erb) have valid syntax, and that \*.pp files pass a puppet-lint check. You may
need to adjust the PATH declared in the script to suit your environment.
