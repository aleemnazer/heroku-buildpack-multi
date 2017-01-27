Usage

To use this buildpack, you should prepare .buildpacks file that contains this buildpack url and your real buildpack url.

$ ls
.buildpacks
...

$ cat .buildpacks
https://github.com/aleemnazer/heroku-buildpack-multi
https://github.com/heroku/heroku-buildpack-play

$ heroku buildpacks:add https://github.com/aleemnazer/heroku-buildpack-multi

$ git push heroku master
...

You can verify installing ffmpeg by following command.

$ heroku run "ffmpeg -version"


For more details about multiple buildpacks

You can also check out Heroku's [built-in buildpack-multi support](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app).