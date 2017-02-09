# OMERO

### Commonly used
```sh
# get omero configurations
$ /opt/omero/OMERO.server/bin/omero config get

# start/stop omero server
$ /etc/init.d/omero start
$ /etc/init.d/omero stop
$ /etc/init.d/omero status 

# start/stop omero web server
$ /etc/init.d/omero-web start
$ /etc/init.d/omero-web stop
$ /etc/init.d/omero-web status 

```


### LDAP / Active Directory

```sh
# do ldap/ad search using shell script wrapper
$ /usr/local/sbin/ldapsearch-ad-gc email=email@email.com
$ /usr/local/sbin/ldapsearch-ad-gc email=email@email.com | grep department

# do ldap/ad search using ldap utility
$ ldapsearch -H ldap://<ldapserver>:<port> -D "<ldap-bind-dn>" -w "<ldap-bind-password>" -b "<base-dn-for-search>" "<email-address>"

```
