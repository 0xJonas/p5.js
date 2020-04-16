# 🌸欢迎！🌺
感谢你为p5.js做出的贡献！我们的团队重视每一种形式的帮助，并且正在尽可能的扩大帮助的范围，包括文件、教学、编写程序、创作艺术、写作、设计、活动、组织、助理或者任何你能想象到的东西。[我们的网站](https://p5js.org/community/#contribute)上提供了一些提供帮助与参与项目的方法。如果要提供技术性的帮助，请接着往下读。

本项目遵循[贡献者名单](https://github.com/kentcdodds/all-contributors)。遵循[指示](https://github.com/processing/p5.js/issues/2309)把你和你的贡献添加到[readme](https://github.com/processing/p5.js/blob/master/README.md#contributors)，或者是在[GitHub issue](https://github.com/processing/p5.js/issues)中评论你的帮助，我们就会把你加入到贡献者名单中。

# 源代码

首要的 p5.js 项目包括了一下几个其他的repo：
- [p5.js](https://github.com/processing/p5.js)：包括了p5.js源代码。[面向用户的p5.js参考手册](https://p5js.org/reference/)也是由包含在此源代码中的[JSDoc](http://usejsdoc.org/)生成的。它归[Lauren Lee McCarthy](https://github.com/lmccart)所有。
- [p5.js-website](https://github.com/processing/p5.js-website)：此源代码包含了[p5.js website](http://p5js.org)的大多数代码（除参考手册外）。它归[Lauren Lee McCarthy](https://github.com/lmccart)所有。
- [p5.js-sound](https://github.com/processing/p5.js-sound)：包括了p5.sound.js库。归[Jason Sigal](https://github.com/therewasaguy)所有。
- [p5.js-web-editor](https://github.com/processing/p5.js-web-editor)：包含了[p5.js web editor](https://editor.p5js.org)的源代码。 归[Cassie Tarakajian](https://github.com/catarak)所有。请注意，旧版[p5.js editor](https://github.com/processing/p5.js-editor)已不再支持。
- [p5.accessibility](https://github.com/processing/p5.accessibility)：使p5.js更适合盲人和视障人士使用的库。

# 文件结构

这个repo有很多文件，所以这里提供了文件总览。有些文件可能很难懂——不过在你开始之前，你不需要每一个都看懂。我们建议你先从一个特定领域入手（例如说，修复某些内联文档），并努力地探索更多领域。Luisa Pereira的[Looking Inside p5.js](http://www.luisapereira.net/teaching/looking-inside-p5/)也给出了p5.js工具与文件的视频总览。

- `contributor_docs/` 包含了贡献者所需遵循的原则；
- `docs/` 并不包含文档！它包含了 _*生成*_ [线上参考手册](https://p5js.org/reference/)的代码；
- `lib/` 包含一个空示例和the p5.sound扩展功能，并且会周期性地通过[p5.js-sound repository](https://github.com/processing/p5.js-sound)更新。这里也是当用[Grunt](https://gruntjs.com/)把p5.js编译到单个文件后p5.js的位置。发出Pull request时，无需将其检入GitHub存储库。
- `src/` 包含该库的所有源代码，这些源代码通常组织成多个单独的模块。 如果要更改p5.js，这就是您要进行的工作。 大多数文件夹内部都有自己的readme.md文件，以帮助您找到解决方法。
- `tasks/` 包含执行与新版本p5.js的构建，部署和发行有关的自动化任务的脚本。
- `tests/` 包含单元测试，这些单元测试可确保库随着更改而继续正常运行。
- `utils/` 可能包含对存储库有用的其他文件，但是通常您可以忽略此目录。
