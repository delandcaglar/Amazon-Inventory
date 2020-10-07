# Amazon Inventory Helper

## Description

Currently Amazon seller manages inventory in google sheets. Python orders parser is implemented and launched from Excel. Program parses all new loaded orders and outputs excel helper file to reduce inventory from the items sold.

Project is heavily based on [previous work](https://github.com/yomajo/Amazon-Orders-Parser).

### Project Caveats:

* Not uploading source files, or databases due to sensitivity of personal information;
* No Excel side (VBA) implementation is uploaded;

## Features

* Filters out orders already processed before (present in database)
* Logs, backups database;
* Automatic database self-flushing of records as defined by `ORDERS_ARCHIVE_DAYS` in [orders_db.py](https://github.com/yomajo/Amazon-Inventory/blob/master/Helper%20Files/orders_db.py);
* Creates a helper file to aid inventory management.

## Output File Sample

Example of output helper excel file:

![Output file sample]()


## Requirements

**Python 3.7+** 

``pip install requirements.txt``