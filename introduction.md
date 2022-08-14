# 引言
感谢你下载这本书！
接下来我们将通过 11 个章节完成一个`Phaser 3`的游戏开发。 在这一过程中我们会使用`TypeScript`, 而我们要开发的游戏是一个类似于《疯狂喷气机》（*Jetpack Joyride*）的无限奔跑的游戏。
是的，我们的英雄会有一个喷气背包。
这本书的目标群体是使用`Phaser 3`开发过至少一个游戏或者是已经读过[Infinite Jumper in Phaser 3 with Modern JavaScript book](https://ourcade.co/books/infinite-jumper-phaser3)这本书的开发者。
我们不会涉及`TypeScript`的基础，但是你可以通过[TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/)来学习。
我们将会带你一步一步的使用`TypeScript`而不是`JavaScript`制作`Phaser 3`游戏。
另外，`Phaser 3` 官方是有`TypeScript`支持的，但是`TypeScript`的经验有时是靠不住的，甚至这些经验会对刚接触`Phaser`框架或`Typescript`的新手带来困惑。
使用`TypeScript`的开发中可能存在一些尴尬的情况，有些写法在`JavaScript`中没有问题，但是在`Typescript`中不被允许。
我们将会为你展示解决这些问题的方法，这些方法恰恰基于`TypeScript`的静态分析能力和其他一些特性，而这些特性也正是让`Typescript`在一些大的代码库里流行的原因。
## 为什么用`TypeScript`

`TypeScript`作为`Microsoft`的开源项目首次发布于2012年。`TypeScript` 多年来只是慢慢地扩散,直到2019年才真正流行起来。
越来越多的专业团队和开源项目都在使用`TypeScript`，让我们有理由关注它。
`Phaser 4` 现在位于早期的开发阶段，它也在使用`TypeScript`。

这些算是使用`TypeScript`的明确动机了，如果这些对于你来说还不够充分，那么接下来我们再来看看使用`Typescript`的收益吧。

`TypeScript` 可以让你现在就用上`JavaScript`语言的现代特性。这些特性是当下被设计进`JavaScript`里面去的，用了`TypeScript`后你就不需要等待浏览器支持或者等用户更新浏览器然后才能使用这些新特性。

这些特性包括 `private` 或 `public` 的访问修饰符，`async/await`，可选链，泛型和更多的存在于其他语言的特性，这些语言有C#、Swift、Kotlin 等。

这些特性还包括类型安全，它可以让你写出更容易维护、更新和使用的代码————包括你自己未来的版本。

如果你有过修改老的`JavaScript`项目的经历，那么光是弄清楚传递的数据长什么样就要花几个小时。`TypeScript`可能会是你新的好朋友。

`TypeScript`使用静态类型解决了这个问题，静态类型提供了数据结构的信息，你不再需要依赖于注释去了解数据是怎么组织的，也不需要担心注释是不是最新的。

使用`TypeScript`开发`Phase 3`游戏也有很多的收益，但我们不想再罗列这些了。

事实是当你拿起这本书你可能已经被`TypeScript`说服了，所以让我们开始使用它吧。

## 如何使用这本书

这本书旨在让你从头到尾地阅读并跟着实践的。
它不是一本参考书可以简单跳过。
每个章节都是建立在前面的内容和复杂度之上的，而这个复杂度也随着你的进步在增加。
这本书的目标是构建一个可运行的游戏，你可以轻松地修改这个游戏也可以加上自己的功能。

## 源代码
你可以在`Github`上下载这个游戏的全部代码：
[https://github.com/ourcade/infinite-runner-template-phaser3](https://github.com/ourcade/infinite-runner-template-phaser3)
这个仓库使用了`git-lfs`所以你需要安装它之后，才可以使用使用`git clone`拉取代码或者图片资源。

或者，你也可以直接下载一个`zip`文件。

我们打算通过增量更新来改进这本书。你可以随时让我知道书里的任何错误、不清楚的说明或者其他的问题，我们的邮件是[tommy@ourcade.co](mailto:tommy@ourcade.co)，也可以使用[Twitter@ourcadehq](http://twitter.com/ourcadehq)

现在让我们制作一个游戏吧，怎么样？
>Ourcade 是一个有趣的游戏开发社区，面向开发和乐观的学习者和开发者。[访问我们](http://ourcade.co)
