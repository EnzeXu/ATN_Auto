
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
| python3.5 / 3.6 / 3.7 / 3.8 | Linux / Windows / MacOS | Both OK |

****
# Catalog

* [1 Purpose](#1-purpose)
* [2 Compile & Execution Instructions](#2-compile--execution-instructions)

****

# 1 Purpose

1. Auto test for DPS model on ATN datasets.

****

# 2 Build Virtual Environment
```shell
$ sudo pip3 install virtualenv
$ cd ~
$ virtualenv atn_auto
```

# 3 Cloning & Executing Instructions
```shell
$ source ~/atn_auto/bin/activate # activate virtual environment
(atn_auto) $ pip list # should be very few packages here
(atn_auto) $ cd ~/workspace
(atn_auto) $ git clone https://github.com/EnzeXu/ATN_Auto.git
(atn_auto) $ cd ATN_Auto
(atn_auto) $ tar jxvf data/atn_data_x_n.tar.bz2 # IMPORTANT
(atn_auto) $ pip install -r requirements.txt
(atn_auto) $ python3 auto.py 1 test # python auto.py {times_of_loop} {any_comments}
# It is normal to see huge warnings at this step, but don't worry.
# after it finishes (1 times may cost several minutes)
(atn_auto) $ cat record/record.csv
(atn_auto) $ deactivate
```
