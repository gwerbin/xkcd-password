## Why did you make this?

Because I didn't know about [XKPasswd](https://xkpasswd.net/s/) until after I 
already wrote the script.

## Requirements

- Zsh > 5.0.8 (the one that ships with macOS 10.11 / i.e. Darwin 15)
- Unix-alike operating system (i.e. paths use forward slashes) with the `xxd`, `fold`, 
  `xargs`, and `printf` commands, as well as the `/dev/random` device.
- the following files in `/usr/share/dict`: `words`, `web2a`, and `propernames`.

## Instructions

Download the file `password` and execute it:
```
./password $n_tokens
```

where `$n_tokens` is the number of phrases you'd like to include. For example:
```
./password 5
```

might generate

```
quarter_bill toxiphoric world-confounding prorector jelly_roll
```

## Development

Toss out a PR if you want.

### To-Dos

- Specify a password dictionary instead of hard-coding it

## License

This project is licensed under my own "MIT+" license, with copyright year 
2016, available in full at https://raw.githubusercontent.com/gwerbin/oss-license/master/LICENSE.
