# read

> 从标准输入（或文件）读取一行并将单词分配给变量。
> 更多信息：<https://www.gnu.org/software/bash/manual/bash.html#index-read>.

- 读取键盘输入的数据赋值给变量：

`read {{变量}}`

- 将您输入的每一行存储为数组一个元素：

`read -a {{数组}}`

- 指定要读取的字符数，将数据赋值给变量：

`read -n {{字符数}} {{变量}}`

- 将多个数据依次赋值给多个变量：

`read {{_ 变量1 _ 变量2}} <<< "{{The surname is Bond}}"`

- 读取键盘输入的数据赋值给变量，不对\进行转义：

`read -r {{变量}}`

- 键盘输入前显示提示语：

`read -p "{{提示语：}}" {{变量}}`

- 静默模式（如果输入来自终端，则不回显字符）读取键盘输入的数据赋值给变量：

`read -s {{变量}}`

- 从标准输入读取每一行进行操作：

`while read line; do {{echo|ls|rm|...}} "$line"; done < {{标准输入|路径/到/文件|...}}`
