# Configuration

`vfox` allows you to change some configurations, all configuration is stored in the `$HOME/.version-fox/config.yaml` file.

::: tip
If you use `vfox` for the first time, an empty `config.yaml` file will be created automatically.
:::

## Proxy Settings

::: tip
Currently only support http(s) proxy protocol
:::

**Format**: `http[s]://[username:password@]host:port`
```yaml
proxy:
  enable: false
  url: http://localhost:7890
```

## Storage Settings

By default, `vfox` stores SDK cache files in the `$HOME/.version-fox/cache` directory.

::: danger !!!
Before configuring, please make sure that `vfox` has write permission to the folder.⚠⚠⚠
:::

```yaml
storage:
  sdkPath: /tmp
```

## Plugin Registry Address


`vfox` will default to retrieve plugins from [vfox-plugins.lhan.me](https://vfox-plugins.lhan.me).

If you want to use **your own registry or third-party mirror registry**, please configure it following:

```yaml
registry:
  address: 'https://vfox-plugins.lhan.me'
```

::: tip Available Mirrors
- https://cdn.jsdelivr.net/gh/version-fox/vfox-plugins/plugins
- https://rawcdn.githack.com/version-fox/vfox-plugins/plugins
  :::
