# CLI plugin commands 

To make plugin installation easier, [CLI Plugin Commands](https://github.com/ostark/craft-plugin-commands) are installed.

This is a tool that lets you install required plugins en mass. Saving the tiresome job of going through and installing each plugin individually in the CMS dashboard.

The available commands are:

## View plugins 

```
./craft plugin/list
```

## Installing plugins

To install all plugins in one command or install a single plugin:
```
php craft plugin/install ALL
php craft plugin/install <plugin-name>
```

## Uninstalling plugins

In the same way as installing all or single plugins:
```
php craft plugin/uninstall ALL
php craft plugin/uninstall <plugin-name>
```

## Enabling & disabling plugins

In the same way as installing & uninstalling all or single plugins are managed, you can enable or disable plugins:
```
php craft plugin/enable ALL
php craft plugin/enable <plugin-name>

php craft plugin/disable ALL
php craft plugin/disable <plugin-name>
```

