my-cheatsheets for cheat
========================

* Cheat sheet repository for [cheat](https://github.com/cheat/cheat) for myself
* After `git clone`, need to set [Cheatpaths](https://github.com/cheat/cheat#cheatpaths) in conf.yml


Installation
------------

```shell
$ mkdir -p ~/.config/cheat/cheatsheets && cheat --init > ~/.config/cheat/conf.yml
$ cd .config/cheat

$ git clone git@github.com:cheat/cheatsheets.git community
$ git clone git@github.com:umi-uyura/mycheatsheets.git personal
```

Edit .config/cheat/conf.yml

```yaml
cheatpaths:
  - name: personal
    path: /home/<user>/.config/cheat/cheatsheets/personal/cheatsheets
```

Truble shooting
---------------

### [failed to write to pager: exec: "PAGER_PATH": executable file not found in $PATH](https://github.com/cheat/cheat/issues/721)

In conf.yml

`pager: PAGER_PATH` --> `pager: less -FRX`
