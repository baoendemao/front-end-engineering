##### nodemon
nodemon可以监控文件的变化，从而重启server.js，从而实现热更新。<br/>
如nodemon -w server --exec  "node server/server.js "，nodemon监控文件夹server的变化，重启node服务。具体用法如下：

```
$ nodemon -h
  Usage: nodemon [options] [script.js] [args]

  Options:

  --config file ............ alternate nodemon.json config file to use
  -e, --ext ................ extensions to look for, ie. js,jade,hbs.
  -x, --exec app ........... execute script with "app", ie. -x "python -v".
  -w, --watch path.......... watch directory "path" or files. use once for
                             each directory or file to watch.
  -i, --ignore ............. ignore specific files or directories.
  -V, --verbose ............ show detail on what is causing restarts.
  -- <your args> ........... to tell nodemon stop slurping arguments.

  Note: if the script is omitted, nodemon will try to read "main" from
  package.json and without a nodemon.json, nodemon will monitor .js, .mjs, .coffee,
  and .litcoffee by default.

  For advanced nodemon configuration use nodemon.json: nodemon --help config
  See also the sample: https://github.com/remy/nodemon/wiki/Sample-nodemon.json

  Examples:

  $ nodemon server.js
  $ nodemon -w ../foo server.js apparg1 apparg2
  $ nodemon --exec python app.py
  $ nodemon --exec "make build" -e "styl hbs"
  $ nodemon app.js -- --config # pass config to app.js

  All options are documented under: nodemon --help options

```