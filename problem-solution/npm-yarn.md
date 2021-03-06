## npm related


#### npm发部带scope的包
先在 package.json 中 name 中指定 '@scopeName/packageName', 然后在发布的时候需要指定 --access public 选项 `npm publish --access public`

#### Node version management

```
// 安装
npm install -g n

// Use or install the latest official release:
n latest

// Use or install the stable official release:
n stable

// Use or install the latest LTS official release:
n lts
```

#### npm 跟 yarn 命令比较

其中 packageName 代表包的名称

- `npm install == yarn / yarn install`
- `npm install packageName --save == yarn add packageName`
- `npm install packageName --save-dev == yarn add packageName --dev`
- `npm uninstall packageName --save == yarn remove packageName`
- `npm update == yarn upgrade`
- `npm install packageName -g == yarn global add packageName`

#### npm 配置仓库地址

```
// 淘宝地址
npm config set registry https://registry.npm.taobao.org

//当你想发布自己的包时，需要将地址修改回来
npm config set registry https://registry.npmjs.org/
```

#### npm 常用命令

```
//安装包并保存到package.json文件中的devDependencies属性中
npm install packageName --save-dev
or
npm install packageName -D

//安装包并保存到package.json文件中的dependencies属性中
npm install packageName --save

//全局安装一个包
npm install packageName -g

//npm升级自身
npm install npm -g
```
