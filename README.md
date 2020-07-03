# jekyll-travis-deploy-template

Automated script for deployment Jekyll sites via FTP and Travis CI.

## Available scripts
```
script/
+--bootstrap - basic setup of repository
+--build - build script for Jekyll
+--cibuild - CI build script
+--cideploy - CI deployment script
+--server - launch Jekyll server
```

## How to use

### Terminal
```bash
$ apt-get update && apt-get upgrade
$ apt-get install ncftp
$ export JEKYLL_ENV=production
$ export HOST=[FTP server]
$ export PORT=[FTP port]
$ export USERNAME=[FTP username]
$ export PASSWORD=[FTP password]
$ export PROJECT=[project name]
$ script/cibuild
$ script/cideploy
```

### Travis CI
Look at [example](.travis.yml).

## License
[MIT](LICENSE)

Script for deployment was adapted from [this](https://ajaykarwal.com/deploying-jekyll-using-travis-ci) site.
