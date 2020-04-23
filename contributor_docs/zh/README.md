

# 🌸欢迎！🌺

感谢你有兴趣为 p5.js 做出贡献！我们的团队重视每一种形式的帮助，并且正在尽可能的扩大你能帮助的范围，这包括了参考文献、教学、编写程序、创作艺术、写作、设计、活动、组织、展策或者任何你能想象到的东西。[我们的社群网页](https://p5js.org/community/#contribute)提供了一些贡献与参与项目的方法。如果你要提供技术性的帮助，请接着往下读。

本项目遵循[贡献者名单](https://github.com/kentcdodds/all-contributors)规格。你可遵循[指示](https://github.com/processing/p5.js/issues/2309)把你和你的贡献添加到 [readme](https://github.com/processing/p5.js/blob/master/README.md#contributors)，或者是在 [GitHub issue](https://github.com/processing/p5.js/issues) 中评论你的贡献，我们就会把你加入到贡献者名单中。

# 源代码

p5.js 项目除了这个代码库外还包括了以下几个其他的代码库：

- [p5.js](https://github.com/processing/p5.js)：包括了 p5.js 源代码。[面向用户的 p5.js 参考文献](https://p5js.org/reference/)也是由包含在此源代码中的 [JSDoc](http://usejsdoc.org/) 注解生成的。[Lauren Lee McCarthy](https://github.com/lmccart) 为维持者。
- [p5.js-website](https://github.com/processing/p5.js-website)：此源代码包含了 [p5.js website](http://p5js.org )的大多数代码（除参考文献外）。[Lauren Lee McCarthy](https://github.com/lmccart) 为维持者。
- [p5.js-sound](https://github.com/processing/p5.js-sound)：包括了 p5.sound.js 程式库。[Jason Sigal](https://github.com/therewasaguy) 为维持者。
- [p5.js-web-editor](https://github.com/processing/p5.js-web-editor)：包含了 [p5.js web editor](https://editor.p5js.org) 的源代码。[Cassie Tarakajian](https://github.com/catarak) 为维持者。请注意，旧版 [p5.js editor](https://github.com/processing/p5.js-editor) 已不再受支持。
- [p5.accessibility](https://github.com/processing/p5.accessibility)：使 p5.js 更适合盲人和视障人士使用的程式库。

# 文件结构

这个代码库有很多文件，所以这里提供了文件总览。有些文件可能很难懂——不过你并不需要每一个都看懂才能开始。我们建议你先从一个特定区域入手（例如说，修复某些内联参考文献），并逐渐地探索更多领域。Luisa Pereira 的 [Looking Inside p5.js](http://www.luisapereira.net/teaching/looking-inside-p5/) 也给出了 p5.js 工具与文件的视频总览。

- `contributor_docs/` 包含了贡献者所需遵循的原则；
- `docs/` 并不包含参考文献！它包含了 _*生成*_ [线上参考文献](https://p5js.org/reference/)的代码；
- `lib/` 包含一个空白示例和 p5.sound 扩展程式库，并且会周期性地通过 [p5.js-sound 代码库](https://github.com/processing/p5.js-sound) 更新。这里也是当用 [Grunt](https://gruntjs.com/) 把 p5.js 编译到单个文件后 p5.js 程式库的位置。发出 Pull request 时，无需将其检入 GitHub 代码库。
- `src/` 包含所有的源代码，这些源代码通常组织成多个单独的模块。 如果要更改 p5.js，这就是你需要参考的地方。大多数文件夹内部都有独自的 README.md 文件，以帮助您浏览该文件夹。
- `tasks/` 包含创建 p5.js 与新版本 p5.js 的构建、部署和发行有关的自动化任务的脚本。
- `tests/` 包含单元测试，这些单元测试可确保库随着更改仍继续正常运行。
- `utils/` 可能包含对存储库有用的其他文件，但是通常您可以忽略此目录。


# 参考文献

我们意识到参考文献是这个项目中最重要的部分。不好的参考文献是新用户与新贡献者的最大屏障，让项目不具有包容性。[contributing_documentation.md](./contributing_documentation.md) 页面为开始修改参考文献给出了一个深入的导览。p5.js 的参考文献可以在以下几个地方找到：

- [p5js.org/reference](https://p5js.org/reference/)：由 [inline documentation](./inline_documentation.md) 的源代码生成。它包括了文本描述和参数以及随附的代码片段示例。我们将所有这些内联文献和代码放在一起，以使代码和参考文献保持紧密的联系，并强化这样的思想，贡献参考文献与贡献代码至少同等重要。构建库后，它将检查内联参考文献和示例，以确保它们与代码的行为方式匹配。 要做出贡献，您可以先查看 [inline_documentation.md](./inline_documentation.md) 页面。
- [p5js.org/examples](http://p5js.org/examples) 页面包含更长的示例，这些示例对于学习 p5.js 可能有用。要做出贡献，您可以先查看 [adding_examples.md](https://github.com/processing/p5.js-website/blob/master/contributor_docs/Adding_examples.md)。
- [p5js.org/learn](https://p5js.org/learn) 页面包含可帮助您学习 p5.js 和编程概念的教程。 要做出贡献，您可以先查看 [p5.js guide to contributing to tutorials](https://p5js.org/learn/tutorial-guide.html)。
- 您可能会注意到 p5.js 网站目前支持几种不同的语言。这称为国际化（i18n）。您可以在 [i18n_contribution](https://github.com/processing/p5.js-website/blob/master/contributor_docs/i18n_contribution.md)页面了解更多。

# GitHub Issue 流程

* 我们使用 [GitHub issue](https://github.com/processing/p5.js/issues) 跟踪已知的错误和预期的新功能。[Issue lables](./issue_labels.md) 用于将问题分类，例如[适合初学者](https://github.com/processing/p5.js/labels/level%3Abeginner)的问题。

* 如果您想开始处理现有问题，请对你打算探查的问题发表评论，以便其他贡献者知道该问题正在处理中并可以提供帮助。

* 完成有关此问题的工作后，请针对 p5.js master 分支[提交 Pull request](./preparing_a_pull_request.md) 。在PR的描述字段中，包括 “resolves #XXXX” 标记，以解决您要解决的问题。如果 PR 并不能完全解决该问题（即，在PR合并后该问题应保持打开状态），请输入 “addresses #XXXX”。

* 如果发现错误或有想要添加新功能的主意，请先提交问题。请不要直接地提交包含修复程序或新功能的 Pull Request，而不先发出问题，否则我们将无法接受该 Pull Request。在有关该问题获得反馈并得到同意解决该问题后，您可以按照上述过程以提供修复或功能。

* 您可以对问题进行分类，其中可能包括复制错误报告或要求提供重要信息，例如版本号或复制说明。 如果您想开始分类问题，一种简单的入门方法是[在 CodeTriage 上订阅 p5.js](https://www.codetriage.com/processing/p5.js)。[![Open Source Helpers](https://www.codetriage.com/processing/p5.js/badges/users.svg)](https://www.codetriage.com/processing/p5.js)

* [organization.md](https://github.com/processing/p5.js/blob/master/contributor_docs/organization.md) 文件提供了有关如何组织问题以及决策过程的高级概述。如果您有兴趣，欢迎您参与。


# 开发过程

我们知道开发过程可能会有点难——不只是你一个人，所有人一开始都会这么觉得。你可以遵循下面的步骤来设置；如果遇到了问题，你可以在[论坛](https://discourse.processing.org/c/p5js)上讨论或发布一个关于你的问题的 [issue](https://github.com/processing/p5.js/issues)，我们会尽力帮助你的。

1. 下载 [node.js](http://nodejs.org/)（同时将会自动下载 [npm](https://www.npmjs.org) 程式包管理器）

2. 将 [p5.js 代码库](https://github.com/processing/p5.js) [fork](https://help.github.com/articles/fork-a-repo) 到你的 GitHub 账号

3. [复制](https://help.github.com/articles/cloning-a-repository/) 此代码库的新 fork 到本地电脑：

   ```
   $ git clone https://github.com/您的用户名/p5.js.git
   ```

4. 导航到项目文件夹，并使用 npm 安装其所有所需的程式包。

   ```
   $ cd p5.js
   $ npm ci
   ```

5. [Grunt](https://gruntjs.com/) 需要被安装，您可以使用它从源代码构建程式库。

   ```
   $ npm run grunt
   ```

   如果您要不断更改库中的文件，您可以运行 `npm run dev` 以便在源文件发生任何更改时自动为您重建程式库，而无需手动键入命令。

6. 在本地源代码更改然后用 Git [commit](https://help.github.com/articles/github-glossary/#commit) 它们。

   ```
   $ git add -u
   $ git commit -m "YOUR COMMIT MESSAGE"
   ```

7. 再次运行 `npm run grunt` 确保没有语法错误，测试失败或其他问题。

8. 将您对 GitHub 上的 fork 上载（[Push](https://help.github.com/articles/github-glossary/#push)）新更改。

   ```
   $ git push
   ```

9. 一切准备就绪后，使用 [pull request](https://help.github.com/articles/creating-a-pull-request) 发布。

# Gotchas
*待续*