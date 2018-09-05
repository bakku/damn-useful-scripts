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

## License

Use them, change them, delete them. Do what you want with them !
