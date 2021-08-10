# 280blocker-filter-redirector-for-heroku
Allow access to 280blocker filter with the same URL.
This app is designed to deploy on heroku.

# Dependency
- Docker
- Docker Compose
- Heroku CLI

# Deploy
```
heroku login
heroku create
heroku container:login
heroku container:push web -a <APP>
heroku container:release web -a <APP>
```

# Usage
| URL                                   | Redirect Destination                                         |
|---------------------------------------|--------------------------------------------------------------|
| https://<APP>.herokuapp.com/adblock   | https://280blocker.net/files/280blocker_adblock_YYYYMM.txt   |
| https://<APP>.herokuapp.com/domain_ag | https://280blocker.net/files/280blocker_domain_ag_YYYYMM.txt |

