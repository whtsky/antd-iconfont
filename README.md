For use Ant Design's iconfont without alicdn.

## Install

```bash
yarn add @whtsky/antd-iconfont
```

## Usage

In your webpack config:

```js
{
  test: /\.less$/,
  loader: [
    {
      loader: require.resolve('css-loader'),
    },
    {
      loader: require.resolve('less-loader'),
      options: {
        modifyVars: {
          '@icon-url':'"~@whtsky/antd-iconfont/iconfont"'
        },
        javascriptEnabled: true,
      },
    },
  ]
}
```
