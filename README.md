# OpenWrt luci feed

## Description
这个是Clone 981213的一个源，因为自己要编译，所以做一些修改或者添加

## Usage

* 进入源码目录，编译 feeds.conf.def
* 注视掉原有的 src-git luci https://git.lede-project.org/luci
* 添加 src-git luci https://github.com/joole/luci-1

This feed is enabled by default. Your feeds.conf.default (or feeds.conf) should contain a line like:
```
src-git luci https://github.com/openwrt/luci.git
```

To install all its package definitions, run:
```
./scripts/feeds update luci
./scripts/feeds install -a -p luci
```

## API Reference

You can browse the generated API documentation [directly on Github](http://htmlpreview.github.io/?http://raw.githubusercontent.com/openwrt/luci/master/documentation/api/index.html).

## Development

Documentation for developing and extending LuCI can be found [in the Wiki](https://github.com/openwrt/luci/wiki)

## License

See [LICENSE](LICENSE) file.
 
## Package Guidelines

See [CONTRIBUTING.md](CONTRIBUTING.md) file.
