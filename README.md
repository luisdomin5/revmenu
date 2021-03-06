# ![revmenu](https://raw.githubusercontent.com/passy/revmenu/master/assets/logo.png)

[![crates.io](https://img.shields.io/crates/v/revmenu.svg)](https://crates.io/crates/revmenu)
[![Build Status](https://travis-ci.org/passy/revmenu.svg?branch=master)](https://travis-ci.org/passy/revmenu)

revmenu can be used with your terminal multiplexer or as stand-alone tool to
select and check out any hash-like string of characters in the output.

## Usage

This is best used when combined with a terminal multiplexer. For tmux,
there is a [plugin available](https://github.com/passy/tmux-revmenu).

Install via tpm:

```tmux
set -g @plugin 'passy/tmux-revmenu'
```

![demo gif](https://raw.githubusercontent.com/passy/revmenu/master/assets/demo.gif)

### Manual Usage

`revmenu` can read from files and from stdin by passing `-` instead of
a filename.

```
$ git log | head -n 20 | revmenu -
```

## Installation

```bash
$ cargo install revmenu
```

## License

[MIT](LICENSE)
