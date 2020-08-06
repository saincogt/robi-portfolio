When trying to run `yarn dev`, getting error msg.
Find a temp solution metioned in: https://github.com/gatsbyjs/gatsby/pull/25720

Modify `node_modules/gatsby/dist/utils/gatsby-webpack-virtual-modules.js`:

```js
// modify line 18
// const VIRTUAL_MODULES_BASE_PATH = `_this_is_virtual_fs_path_`;
const VIRTUAL_MODULES_BASE_PATH = `node_modules`;
```
