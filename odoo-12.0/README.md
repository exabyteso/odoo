[![Build Status](http://runbot.odoo.com/runbot/badge/flat/1/master.svg)](http://runbot.odoo.com/runbot)
[![Tech Doc](http://img.shields.io/badge/master-docs-875A7B.svg?style=flat&colorA=8F8F8F)](http://www.odoo.com/documentation/master)
[![Help](http://img.shields.io/badge/master-help-875A7B.svg?style=flat&colorA=8F8F8F)](https://www.odoo.com/forum/help-1)
[![Nightly Builds](http://img.shields.io/badge/master-nightly-875A7B.svg?style=flat&colorA=8F8F8F)](http://nightly.odoo.com/)

Odoo
----

Odoo is a suite of web based open source business apps.

The main Odoo Apps include an <a href="https://www.odoo.com/page/crm">Open Source CRM</a>,
<a href="https://www.odoo.com/page/website-builder">Website Builder</a>,
<a href="https://www.odoo.com/page/e-commerce">eCommerce</a>,
<a href="https://www.odoo.com/page/warehouse">Warehouse Management</a>,
<a href="https://www.odoo.com/page/project-management">Project Management</a>,
<a href="https://www.odoo.com/page/accounting">Billing &amp; Accounting</a>,
<a href="https://www.odoo.com/page/point-of-sale">Point of Sale</a>,
<a href="https://www.odoo.com/page/employees">Human Resources</a>,
<a href="https://www.odoo.com/page/lead-automation">Marketing</a>,
<a href="https://www.odoo.com/page/manufacturing">Manufacturing</a>,
<a href="https://www.odoo.com/page/purchase">Purchase Management</a>,
<a href="https://www.odoo.com/#apps">...</a>

Odoo Apps can be used as stand-alone applications, but they also integrate seamlessly so you get
a full-featured <a href="https://www.odoo.com">Open Source ERP</a> when you install several Apps.


Getting started with Odoo
-------------------------
For a standard installation please follow the <a href="https://www.odoo.com/documentation/master/setup/install.html">Setup instructions</a>
from the documentation.

Then follow <a href="https://www.odoo.com/documentation/master/tutorials.html">the developer tutorials</a>

Running the application on a Unix Client:
1. Download this repo onto your client.
2. Install virtualenvwrapper if you don't have it.
  *sudo apt install virtualenvwrapper
  source /usr/share/virtualenvwrapper/virtualenvwrapper.sh*
3. Install the tools required to build Odoo dependencies
  *sudo apt install build-essential python3-dev libxslt-dev libzip-dev libldap2-dev libsasl2-dev*
4. Create an isolated environment for Odoo
  *mkvirtualenv -p /usr/bin/python3 odoo-venv*
5. Install the Odoo's Python dependencies
  *cd your_odoo_sources_path
  pip install -r requirements.txt*
6. To leave the virtual environment execute the command *deactivate*
7. To reactivate the virtual environment execute *workon odoo-venv*
8. Run Odoo using:
  *./odoo-bin --addons-path=addons --db-filter=odoo*

How to create a new module:
odoo-bin scaffold *module name where to put it*

Following https://www.cybrosys.com/blog/how-to-create-module-in-odoo12 tutorial
