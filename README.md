# Heroku App

for testing to do on [heroku](https://jp.heroku.com).  
This repository is sand-box.

## build this app.

use gradle.
```shell
gradlew clean build
```

## init to do use heroku

read [tutorial page](https://devcenter.heroku.com/ja/articles/getting-started-with-gradle-on-heroku
).  
- create heroku account (if do not have this account)
- get `heroku` command
- heroku login
- change dir to working dir (which cloned this repository)  
- do command `heroku create`
- git push (heroku master)
can deploy app to heroku.  
check to run, I should do command `heroku open` or access to heroku web site.

## command for heroku

- buildpack

add
```shell
heroku buildpacks:add heroku/gradle
```

remove
```shell
heroku buildpacks:remove heroku/gradle
```

- start/restart/stop

start
```shell
heroku start -s<app_name>
```

stop
```shell
heroku stop -s<app_name>
```
