# ls

> 列出目录中的内容。
> 更多信息：<https://www.gnu.org/software/coreutils/manual/html_node/ls-invocation.html>.

- 列出目录中的文件，每个文件占一行：

`ls -1`

- 列出包含隐藏文件的所有文件：

`ls {{[-a|--all]}}`

- 列出所有文件，如果是目录，则在目录名后面加上「/」：

`ls {{[-F|--classify]}}`

- 列出包含隐藏文件的所有文件信息，包括权限，所有者，大小和修改日期：

`ls {{[-la|--all -l]}}`

- 列出所有文件信息，大小用人类可读的单位表示（KiB, MiB, GiB）：

`ls {{[-lh|-l --human-readable]}}`

- 列出所有文件信息，按大小降序排序：

`ls {{-lSR|-lS --recursive}}`

- 列出所有文件信息，按修改日期从旧到新排序：

`ls {{[-ltr|-lt --reverse]}}`

- 只列出目录：

`ls {{[-d|--directory]}} */`
