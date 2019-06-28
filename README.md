hujitatsu(藤原竜也変換)
---
Converts a sentence to Fujiwara Tatsuya-style or restores it.

### Usage

```shell
$ hujitatsu '紅だァーーーーッ!!'
紅゛だ゛ァ゛ー゛ー゛ー゛ー゛ッ゛!゛!
```

```shell
$ echo '紅だァーーーーッ!!' | hujitatsu
紅゛だ゛ァ゛ー゛ー゛ー゛ー゛ッ゛!゛!
```

```shell
$ hujitatsu -d '紅゛だ゛ァ゛ー゛ー゛ー゛ー゛ッ゛!゛!゛'
紅だァーーーーッ!!
```

```shell
$ echo '紅゛だ゛ァ゛ー゛ー゛ー゛ー゛ッ゛!゛!゛' | hujitatsu -d
紅だァーーーーッ!!
```

```shell
$ hujitatsu -h
hujitatsu version 0.0.1
Usage: hujitatsu [OPTION] [ARGS]

Hujitatsu(Hujiwara Tatsuya) encode or decode ARGS, or standard input, to standard output.
With no ARGS, or when ARGS is -, read standard input.

Options:
    -d, --decode  decode data
    -h, --help    show help
```
