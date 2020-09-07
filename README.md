Fork of sqlite3dbm
==================

This is a fork of the python package **sqlite3dbm** (https://github.com/Yelp/sqlite3dbm). In this repo I fixed some `python3` compatibilities issues due to the following error:

```
    ERROR: Command errored out with exit status 1:
     command: /users/ragagnin/anaconda3/bin/python -c 'import sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-xa65o_d7/sqlite3dbm/setup.py'"'"'; __file__='"'"'/tmp/pip-install-xa65o_d7/sqlite3dbm/setup.py'"'"';f=getattr(tokenize, '"'"'open'"'"', open)(__file__);code=f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-iwkfiump
         cwd: /tmp/pip-install-xa65o_d7/sqlite3dbm/
    Complete output (10 lines):
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "/tmp/pip-install-xa65o_d7/sqlite3dbm/setup.py", line 1, in <module>
        from sqlite3dbm import __version__
      File "/tmp/pip-install-xa65o_d7/sqlite3dbm/sqlite3dbm/__init__.py", line 23, in <module>
        import sqlite3dbm.dbm as dbm
      File "/tmp/pip-install-xa65o_d7/sqlite3dbm/sqlite3dbm/dbm.py", line 197
        def __init__(self, path, flag='r', mode=0666):
                                                   ^
    SyntaxError: leading zeros in decimal integer literals are not permitted; use an 0o prefix for octal integers
    ----------------------------------------
ERROR: Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.
```

Install
-------

You can install this fork of the `sqlite3dbm` package with the following command:

```python3 -mpip install git+https://github.com/aragagnin/sqlite3dbm/```


Documentation
-------

To access the documentation and to check all other issues please see the homepage of the main project:  https://github.com/Yelp/sqlite3dbm
