
ATN_Auto
===========================
This document is the description of work for ATN_Auto

****
 
| Project Name | Authors |
| ---- | ---- |
| ATN_Auto | Enze Xu (xue20@wfu.edu) & Jingwen Zhang (zhanj318@wfu.edu) |

| Version | Date |
| ---- | ---- |
| v1.0 | 11/17/2021 |

| Python Version | Platform | GPU or CPU |
| ---- | ---- | ---- |
| python3.6 / 3.7 / 3.8 | Linux / Windows / MacOS | Both OK |

****
# Catalog

* [1 Purpose](#1-purpose)
* [2 Compile & Execution Instructions](#2-compile--execution-instructions)

****

# 1 Purpose

1. Auto test for DPS model on ATN datasets.

****

# 2 Compile & Execution Instructions
```shell
$ git clone https://github.com/EnzeXu/ATN_Auto.git
$ cd ATN_Auto
$ sudo pip install -r requirements.txt
# python auto.py {times_of_loop} {any_comments}
$ python auto.py 1 test
# It is normal to see huge warnings at this step, but don't need to worry.
# after it finishes (1 times may cost several minutes)
$ cat record/record.csv
```
