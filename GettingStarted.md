# 入门
这本书将介绍制作一个无限奔跑者的游戏，和*Jetpack Joyride*相似，我们的游戏叫做 *Rocket Mouse*。
我们的目标是让穿喷气背包的老鼠尽可能长时间地活下去并收集硬币避开障碍。

如果你是一个`Phaser 3`和`web`开发新手，我们推荐你查看[Infinite Jumper in Phaser 3 with Modern JavaScript](https://ourcade.co/books/infinite-jumper-phaser3/)这本书。

这本书相对那本书更加高级将会使用一般的开发工具像`Node.js`、`NPM` 和命令行。

正如本书的标题已经说明的，我们将会使用`TypeScript`编写代码，这些`TypeScript`代码可以帮助我们更容易推理和维护数年或数月。

## 安装`Node.js` 和 `NPM`
获取`Node.js`最简单的方法是从[https://nodejs.org](https://nodejs.org)直接下载安装。

当然也有其他的方法，我们这里不再讨论。

如果你已经安装了`Node.js` 和 `NPM`，你可以跳过这个部分，去阅读这篇[博文](https://blog.ourcade.co/posts/2019/get-started-phaser3-fast-painless/)。

当你打开`Node.js`下载页面后，选择针对大多数用户的推荐版本。在我们写这本书的时候，这个版本是`v12.16.x`。

对于我们接下来要做的事情来说，选择那个具体的版本并没有什么影响。

下载安装文件，让后安装屏幕上的提示去把`Node.js`安装到你的电脑上。

安装完成后，打开终端或者命令行，运行下面的命令
```batch
node --version
```
如果安装成功，那么终端或命令行里面将会返回`Node.js`的版本号。这也意味着`NPM`也就是`Node`包管理器也安装好了。

让我们验证一下，运行下面的代码
```batch
npm --version
```
这也将会返回一个版本号。需要注意`Node.js`的版本号和`npm`的版本号并不一样，这也是符合预期的。
## 创建项目
我们将会使用`phaser3-typescript-parcel-template`去启动(bootstrap)我们的项目。你可以在[这里](https://github.com/ourcade/phaser3-typescript-parcel-template)找到它。

如果你熟悉`git`，直接把它克隆下来就行了。

如果你不熟悉，你可以把它当作一个`zip`文件下载，点击屏幕上的绿色按钮`Clone or download`即可。

你可以随意把文件夹的名字“`phaser3-typescript-parcel-template`”改成其它像“`rocket-mouse-game`”这类的名字。

这个项目模板使用了`Parcel`作为打包工具和`web`服务器。

如果你已经通过`webpack` 和 `rollup`，`parcel`是和它们类似的工具，只不过`parcel`标榜零配置启动和速度快。

接下来你需要安装`Parcel`，打开命令行运行下面的命令：
```batch
npm install -g parcel-bundler

```
为了确定`parcel`安装成功，运行下面的命令：
```batch
parcel --version
```
命令行会返回一个类似于`1.12.4`的版本号。

现在我们让这个项目可以使用。在命令行打卡项目文件夹，运行下面的命令
```batch
npm install
```
这行命令会安装项目的依赖，像`Phaser 3` 和一些`Parcel`的插件以完成一些一般性的自动化任务。

接下来，运行下面的命令启动开发服务器
```batch
npm run start
```






