# Odoo-17-Development
Odoo ERP is a vast platform to work. It can be used for may purpose, such as; web developing, employee management, sales management, hr management etc.
----
you can configure using this(for source code user):

[options]
admin_passwd = admin
db_host = localhost
db_port = 5432
db_user = cool
db_password = 1234
addons_path = D:\odoo-17.0\addons
xmlrpc_port = 8069



----
or (for nightly download user)
----

[options]
addons_path = C:\odoo17\server\odoo\addons, C:\odoo17\server\custom
admin_passwd = admin
bin_path = C:\odoo17\thirdparty
csv_internal_sep = ,
data_dir = C:\odoo17\sessions
db_host = localhost
db_maxconn = 64
db_maxconn_gevent = False
db_name = False
db_password = openpgpwd
db_port = 5432
db_sslmode = prefer
db_template = template0
db_user = openpg
dbfilter = 
default_productivity_apps = True
demo = {}
email_from = False
from_filter = False
geoip_city_db = c:\usr\share\geoip\geolite2-city.mmdb
geoip_country_db = c:\usr\share\geoip\geolite2-country.mmdb
gevent_port = 8072
http_enable = True
http_interface = 
http_port = 8069
import_partial = 
limit_memory_hard = None
limit_memory_soft = None
limit_request = None
limit_time_cpu = None
limit_time_real = None
limit_time_real_cron = None
list_db = True
log_db = False
log_db_level = warning
log_handler = :INFO
log_level = info
max_cron_threads = 2
osv_memory_count_limit = 0
pg_path = 
pidfile = 
proxy_mode = False
reportgz = False
screencasts = 
screenshots = c:\users\user\appdata\local\temp\odoo_tests
server_wide_modules = base,web
smtp_password = False
smtp_port = 25
smtp_server = localhost
smtp_ssl = False
smtp_ssl_certificate_filename = False
smtp_ssl_private_key_filename = False
smtp_user = False
syslog = False
test_enable = False
test_file = 
test_tags = None
transient_age_limit = 1.0
translate_modules = ['all']
unaccent = False
upgrade_path = 
websocket_keep_alive_timeout = 3600
websocket_rate_limit_burst = 10
websocket_rate_limit_delay = 0.2
without_demo = False
workers = None
x_sendfile = False


----
If you use the second option, you will need to download the other part as <b><i>{}launch.json</i></b>

in that file you will have to write this:

{
    // A Configuration Code For Vs-Code
    "version": "0.2.0",
    "configurations": [{
        "name": "Python: Odoo17",
        "type": "debugpy",
        "request": "launch",
        "stopOnEntry": false,
        "python": "C:\\odoo17\\python\\python.exe",
        "console": "integratedTerminal",
        "program": "${workspaceRoot}\\odoo-bin",
        "args": [
            "--config=${workspaceRoot}\\odoo.conf",
        ],
        "cwd": "${workspaceRoot}",
        "env": {},
        "envFile": "${workspaceRoot}/.env",
        "debugOptions": [
            "RedirectOutput"
        ]
    }]
}




