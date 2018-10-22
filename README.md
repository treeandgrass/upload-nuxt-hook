# upload-nuxt-hook

###
npm i -D upload-nuxt-hook

### 使用
npm install upload-nuxt-hook
const UploadPlugin = require('upload-nuxt-hook')
在nuxt.config.js中配置
async 'generate:done'() {
     await new UploadPlugin({
       root: './dist',
       filterExts: ['.gif', '.js' , '.mp4', '.html', '.css', '.json', '.jpeg', '.png', '.svg', '.ttf', '.eot', '.jpg', '.ico'],
       delayTime: 3000,
       accessId: '',
       secretKey: '',
       endpoint: '',
       port: ,
       bucket: ''
     }).execute()
    }
