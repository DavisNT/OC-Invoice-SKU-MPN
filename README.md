OpenCart 2.3/3.0 Invoice SKU MPN
===============
OpenCart 2.3 and 3.0 modification to display Manufacturer name, SKU and MPN instead of Model in invoices

## Introduction

This modification changes invoices in OpenCart admin interface - adds Manufacturer, SKU and MPN columns, and removes Model column from table of products in the invoice.

This is tested only on OpenCart 2.3.0.2 and OpenCart 3.0.3.8.

## Installation

1. For OpenCart 3.0 inside the folder `Invoice-SKU-MPN_oc30.ocmod` compress `install.xml` into `Invoice-SKU-MPN_oc30.ocmod.zip`.
1. Open Extensions Installer in OpenCart admin interface.
1. On OpenCart 2.3 upload/install `Invoice-SKU-MPN_oc23.ocmod.xml`.
1. On OpenCart 3.0 upload/install `Invoice-SKU-MPN_oc30.ocmod.zip`.
1. Open Modifications in OpenCart admin interface and click Refresh.
1. Edit the language file (e.g. `admin/language/en-gb/sale/order.php`) of your OpenCart installation (e.g. via FTP) and add lines like these: 

```php
$_['column_sku']             = 'SKU';
$_['column_mpn']             = 'MPN';
$_['column_manufacturer']    = 'Manufacturer';
```


## Notices

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
