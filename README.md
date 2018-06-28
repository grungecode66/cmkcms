# cmkcms
Cromaca content management system

## Provisioning

### Architecture

  - 3 GB Ram
  - 60 GB Storage (wo nfs) 20 GB (with nfs)


### Dependencies

  - Ubuntu-16.04
  - Apache2
  - PHP
  - Mysql
  - ffmpeg
  - nfs-client
  - phpmyadmin
  - python-mysql
  - git
  - vim


### Configuration

#### Apache2
- use password in this version in apache conf
- sites-enabled and available pointing to /srv/webroot
- proper mods for php and mysql

#### MySql
- non-root user
- if local no remote access needed


### Application Layout

/srv/webroot/cmkcms
            app/
              web application code
            doc/
            log/
            provision/
            tools/
            fs/ (nfs mounted or local storage)
            

### Use

At the bare minimum a web server should be up and running to access the content via browser.

The next step would be to all access to a database that contains info about the items in the fs.

Additionally it would be helpful to keep the items in the db and the fs synced.

As icing on the cake, a crud application should be available for the data/content.

Nirvana would be reporting, filtering and tagging data

























