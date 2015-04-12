

# Setup

### `ENV` VARIABLES
* `PROX_GEM_GIT_URI=https://git@github.com/sinatra`
* `PROX_GEM_MODE=git`


# Tags

As I worked toward getting this working, I tagged some commits.  Here are the names and how they did

* `prox_gem_file` - Can't parse
* `prox_gem_inlined` - Works fine
* `prox_gem_require_relative_proper_path` - Can't parse
* `require_using_load_path_modification` - Works fine

## Can't Parse Error Message

```
☺ ~/code/heroku-prox-gem-test[master]% git push heroku
Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 480 bytes | 0 bytes/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote:
remote: -----> Ruby app detected
remote: -----> Compiling Ruby/Rack
remote:  !
remote:  !     There was an error parsing your Gemfile, we cannot continue
remote:  !     There was an error in your Gemfile, and Bundler cannot continue.
remote:  !
remote:
remote:  !     Push rejected, failed to compile Ruby app
remote:
remote: Verifying deploy...
remote:
remote: ! Push rejected to boiling-harbor-9776.
remote:
To https://git.heroku.com/boiling-harbor-9776.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://git.heroku.com/boiling-harbor-9776.git'
```
