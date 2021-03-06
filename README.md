# Damn Useful Scripts

Just a list of scripts that grants a dev (like me) a happier life.

Coding guidelines:

- Must be one-liners
- As complex as possible
- No mutable variables, only combination of tools/method sequences

### pj

Commandline JSON prettifier

```
$ pj '{"this_json_is":"ugly"}'
{
  "this_json_is": "ugly"
}
```

### gpass

Password generator (because rake/rails secret is slow and I don't want to leave the terminal for [http://passwordsgenerator.net/](http://passwordsgenerator.net/))

```
$ gpass 32
IBOLsHI96AhxdDldZETnTHWC8jnIdUkJ
```

### objectid

ObjectID generator in case you need them often for sample data

```
$ objectid
5b8fb395a595f1824326425f
```

### lorem

Generates a random paragraph using [https://baconipsum.com/json-api/](https://baconipsum.com/json-api/).

```
$ lorem
Rump andouille shankle, minim corned beef picanha eu drumstick commodo quis in labore et. Shankle cow turkey velit pancetta chuck sirloin. Frankfurter kevin adipisicing, ball tip tail corned beef tenderloin jowl kielbasa bresaola brisket burgdoggen do incididunt. Cillum elit qui shoulder.
```

### clj-try

Want to try some clojure lib in a REPL session? Use `clj-try`:

```
$ clj-try medley "1.3.0"
Downloading: medley/medley/1.3.0/medley-1.3.0.pom from clojars
Downloading: medley/medley/1.3.0/medley-1.3.0.jar from clojars
Clojure 1.10.1
user=> (require '[medley.core :as m])
nil
user=> (m/find-first even? [1 2 3 4])
2
```

### serve

Start a file server and serve the current directory on port 9090 (requires WEBrick).

```
$ serve 
[2021-03-25 14:42:35] INFO  WEBrick 1.7.0
[2021-03-25 14:42:35] INFO  ruby 3.0.0 (2020-12-25) [x86_64-darwin20]
[2021-03-25 14:42:35] INFO  WEBrick::HTTPServer#start: pid=63180 port=9090
```

### smtptest

Check whether a smtp account works properly (requires mail gem).

```
$ smtptest mail.server.com sender@example.com password recipient@example.com
```

## License

Use them, change them, delete them. Do what you want with them !
