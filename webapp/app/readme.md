# 導入

## コマンド

* yarn global add @vue/cli
* vue create プロジェクト名
* custom
* typescript
* cd プロジェクト名
* vue.config.jsを作成
  * コンテナ内などだとhotreloadが効かない場合があるらしい。
  必要ならpollingを設定する。
　vueのversionによって設定が異なるため注意

  ```js
  const { defineConfig } = require('@vue/cli-service')
  module.exports = defineConfig({
    transpileDependencies: true,
    configureWebpack: {
      watchOptions :{
        aggregateTimeout: 300,
        poll: 1000
      }
    }
  })
  ```

* yarn add bootstrap @popperjs/core
* yarn serve

