---
title: Setting Up My Ubuntu
excerpt: Post install script, software settings.
published: true
date: 2019-06-24
categories: project
tags: bash
---

## Installing Windows

### Foobar
``` bashcd 
[https://www.foobar2000.org/encoderpack]
foo_discogs
foo_dsd_processor
foo_input_dts
foo_dsp_xgeg
foo_input_monkey
foo_input_sacd
foo_out_upnp
foo_upn
```



## Installing Ubuntu

### Disk Partition Size

``` bash
+---------+-----------+----------+
|  DISK   | PARTITION |   SIZE   |
|---------+-----------+----------|
|   SSD   |     /     |   40 Gb  |
|         |    swap   |   12 Gb  |
|   HDD   |   /home   |   15 Gb  |
+---------+-----------+----------+
```

Regain ownership of all files run this:

``` bash
sudo chown -R hsunwei /home/hsunwei
```

### Chinese input

1. System Settings–>Language Support–>Install/Remove Languages
2. `sudo apt-get install ibus ibus-clutter ibus-gtk ibus-gtk3 ibus-qt4`
3. `sudo apt-get install ibus-pinyin`
4. Logout
5. sudo ibus-setup


### Installing Anaconda

[Anaconda Distribution Download](https://www.anaconda.com/distribution/)
[Recommended change to enable conda in your shell](https://github.com/conda/conda/releases/tag/4.4.0)



### Useful software
- [Youtube downloader](https://github.com/rg3/youtube-dl/blob/master/README.md#options)
`youtube-dl --write-auto-sub https://www.youtube.com/playlist?list=PLLssT5z_DsK-h9vYZkQkYNWcItqhlRJLN`
- [Kindle-friendly pdf converter](http://www.willus.com/k2pdfopt//)
`k2pdfopt *.pdf -dev kp3`


- [HTML 5 outliner for Chrome](https://h5o.github.io/) [HeadingsMap for Firefox](https://addons.mozilla.org/en-US/firefox/addon/headingsmap/) [How can I add a table of contents to an ipython notebook?](https://stackoverflow.com/questions/21151450/how-can-i-add-a-table-of-contents-to-an-ipython-notebook)

### Post install script

{% gist 4ca47b320b0f7e13a16958210eef034c %}