Simplest possible hello world heroku node.js app that uses middleware

- Here is the github repo : https://github.com/ogt/helloworld-js-heroku-depends
- Here is the heroku app : http://guarded-stream-2218.herokuapp.com/  (20+ sec delay at first fetch)
- Here is the blog post about this : http://otdump.blogspot.com/2013/02/work-notes-using-middlewares.html

Run locally as
```
> # assumes installed github hub, heroku toolbelt
> repo=helloworld-js-heroku-depends
> hub fork ogt/$repo
> hub clone $repo
> cd $repo
> foreman start
> open http://localhost:5000
```
Run on heroku as

```
> # assumes in $repo folder, local changes commited, already done the run local above
> heroku login
> heroku create $repo
> git push heroku master
> heroku open
```

Previous iteration of this app is https://github.com/ogt/helloworld-js-heroku

Next iteration of this app is https://github.com/ogt/helloworld-node-cookies
