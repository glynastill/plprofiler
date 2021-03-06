Installing PL Profiler
======================

The backend part of the **plprofiler** is a PostgreSQL extension, that compiles with USE_PGXS in the `Makefile`. This means that it can be compiled and installed when checked out into the `contrib` directory of the PostgreSQL source tree.

The **plprofiler** command line utility is a Python module with a main() entry point. It is found in then `plprofiler/python-plprofiler` directory. If you are using Python virtualenv, just run `python ./setup.py install` in that directory. If you do not use virtualenv, the utility needs to be installed in the system wide Python site packages by root:

```
cd python-plprofiler
sudo python ./setup.py install
```
The module requires the psycopg2 database connector. Run whatever is require on your system to install the python-psycopg2 RPM (yum, apt-get, pip, ?").
