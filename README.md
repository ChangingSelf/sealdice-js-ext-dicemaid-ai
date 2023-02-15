# 海豹js扩展-AI骰娘


### 介绍

用来给自己的骰娘接入AI，给骰娘注入灵魂，让她可以和你聊天对话（然而不太聪明的样子）

[如何给你的骰娘接入AI](https://docs.qq.com/doc/DUkpqcFlQSWdjVFVN)


### 如何使用

#### 获取key和bid

在brainshop.ai注册，新建一个大脑，在设置面板即可获得key和bid

#### 编译

clone或下载项目，随后在src目录下新建一个key.ts文件，里面写入：

```ts
export const apiKey = {
    bid: '你的bid',
    key: '你的key'
}

export const diceMaidQQ = '你骰娘的QQ号';

```

在终端使用如下命令进行编译：

```
npm install
npm run build
```

好的，现在你的项目被编译成功了，就在dist目录。

将编译好的js文件上传到海豹骰，就可以使用了。

#### 指令

```
.聊天 你要说的内容
.chat 你要说的内容
@骰娘 你要说的内容
```

