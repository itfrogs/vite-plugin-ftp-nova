# vite-plugin-ftp-nova
a simple useful vite ftp plugin, based on [ftp-deploy](https://github.com/itfrogs/vite-plugin-ftp-nova), upload your dist file after vite build.

# install
```
> npm i vite-plugin-ftp-nova --save-dev
```

# usage

```js
// vite.config.ts
import vitePluginFtp from 'vite-plugin-ftp-nova'

export default {
  plugins: [
    vitePluginFtp({
        host: '127.0.0.1',
        port: 21,
        remoteDir: '/www/wwwroot',
        user: 'root',
        password: '123456',
    })
  ]
}
```