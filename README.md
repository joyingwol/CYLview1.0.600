# CYLview1.6.0

`CYLview v1.0.561 BETA` can no longer check for version updates properly. After entering registration information, the following error will be displayed:

```bash
Exception in Tkinter callback
Traceback (most recent call last):
  File "Tkinter.pyc", line 1403, in __call__
  File "/Users/Claude/workspace/CYLVIEW_PROJECT/cylview/modules/about.py", line 98, in <lambda>
  File "/Users/Claude/workspace/CYLVIEW_PROJECT/cylview/modules/about.py", line 141, in check_for_updates
UnboundLocalError: local variable 'curr_version' referenced before assignment
```

Through Fiddler packet capture, the URLs for checking version updates and registering user information, `https://www.cylview.org/BUILD/subreg.php?body=[information strings]` and `https://www.cylview.org/BUILD/version.txt`, show a 403 Forbidden error. Therefore, it can only be used by obtaining the full version of the new version.

![](https://s2.loli.net/2025/07/17/OvGTCM7xbBV5Iw6.png)

This repository contains the full version of `CYLview v1.6.0 BETA`.

Below is the copyright statement for this software:

```plain
CYLview BETA 1.0
Copyright (C) 2009-2012 Claude Y. Legault
University of Sherbrooke, Canada

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to use the Software as obtained. The above copyright notice and this permission notice shall be included in all copies of the Software.

Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

If this issue is resolved, this repository may be deleted at any time, please be aware.
