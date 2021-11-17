
ATN_Auto
===========================
This document is the description of work for ATN_Auto

****
 
| Project Name | Author |
| ---- | ---- |
| ATN_Auto | Enze Xu (xue20@wfu.edu.cn) & Jingwen Zhang (zhanj318@wfu.edu.cn) |

| Version | Date |
| ---- | ---- |
| v1.0 | 11/17/2021 |

****
# Catalog

* [1 Purpose](#1-purpose)
* [2 Format](#2-format)
* [3 Demo](#3-demo)

****

# 1 Purpose

1. Auto test for DPS model on ATN datasets.

****

# 3 Compile & Execution Instructions
```shell
$ git clone https://github.com/EnzeXu/ATN_Auto.git
$ cd ATN_Auto
$ sudo pip install -r requirements.txt
$ python auto.py test
```

```shell
$ python demo.py
shape = (2, 3)
[ +x1 +2*x2,    +x2 +x3,    +x1 +x3 ]
[       +x1,      +2*x2,      +3*x3 ]

shape = (3, 2)
[    +1,    +y1 ]
[    +2,  +y2^2 ]
[    +3,  +y3^3 ]

shape = (2, 2)
[                                   +4*x1 +4*x2 +5*x3,  +x1*y1 +x1*y3^3 +2*x2*y1 +x2*y2^2 +x3*y2^2 +x3*y3^3 ]
[                                     +x1 +4*x2 +9*x3,                         +x1*y1 +2*x2*y2^2 +3*x3*y3^3 ]

sm3[0][1]:  +x1*y1 +x1*y3^3 +2*x2*y1 +x2*y2^2 +x3*y2^2 +x3*y3^3
```