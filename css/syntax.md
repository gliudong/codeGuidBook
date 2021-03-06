<a name="css-syntax"></a>
## 1. 语法

> “作为成功的项目的一员，很重要的一点是意识到只为自己写代码是很糟糕的行为。如果将有成千上万人使用你的代码，
> 那么你需要编写最具明确性的代码，而不是以自我的喜好来彰显自己的智商。” - Idan Gazit

* 在任何代码库中，无论有多少人参与及贡献，所有代码都应该如同一个人编写的一样。
* 严格执行一致认可的风格。
* 用两个空格来代替制表符（tab） -- 这是唯一能保证在所有环境下获得一致展现的方法。
* 为了代码的易读性，在每个声明块的左花括号前添加一个空格。
* 声明块的右花括号应当单独成行。
* 每条声明语句的 : 后应该插入一个空格。
* 为了获得更准确的错误报告，每条声明都应该独占一行。
* 所有声明语句都应当以分号结尾。最后一条声明语句后面的分号是可选的，但是，如果省略这个分号，你的代码可能更易出错。
* 对于以逗号分隔的属性值，每个逗号后面都应该插入一个空格（例如，box-shadow）。
* 对于属性值或颜色参数，省略小于 1 的小数前面的 0 （例如，.5 代替 0.5；-.5px 代替 -0.5px）。
* 尽量使用简写形式的十六进制值，例如，用 #fff 代替 #ffffff。
* 避免为 0 值指定单位，例如，用 margin: 0; 代替 margin: 0px;。

