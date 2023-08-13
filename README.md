# Welcome to the excel-dw wiki!


* Create Overlay Network `excel-dw-network`

* Create Configs `excel_dw_config` & [copy the excel_dw_config](https://github.com/excel-azmin/excel-dw/wiki/superset_config)

* Create Stack `excel-dw` & [copy the docker-compose](https://github.com/excel-azmin/excel-dw/wiki/docker%E2%80%90compose)

* Set environment variable 

```
VERSION = 2.1.0
MAPBOX_API_KEY = {your key}
SITE = dw.example.com
```

* Enter the superset console and complete the setup

```
# Initialize the database
superset db upgrade

# Create an admin user in your metadata database (use `admin` as username to be able to load the examples)
FLASK_APP=superset superset fab create-admin

# Load some data to play with (Optional)
# superset load_examples

# Create default roles and permissions
superset init

```
