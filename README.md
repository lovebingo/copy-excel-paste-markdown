# Copy Excel Paste Markdown

Copy a table in Excel (or other spreadsheet programs) and paste it as a Markdown table.

![demo](https://cl.ly/120h1K2Q1Y3H/Screen%20Recording%202016-08-31%20at%2010.31%20PM.gif)

## Column Alignments

You can optionally specify column alignment information by prepending one of the following to the column heading names in Excel:

* ^c  - center alignment
* ^r  - right alignment
* ^l   - left alignment (the default)

For example: enter the following in Excel to right-align the second column and center-align the third column:

| animal | ^rweight | ^ccolor  |
|--------|----------|----------|
| dog    | 30lb     | tan      |
| dog    | 85lb     | black    |
| cat    | 18lb     | calico   |

This will produce the following markdown table when pasted:

```markdown
| animal | weight | color  |
|--------|-------:|:------:|
| dog    | 30lb   | tan    |
| dog    | 85lb   | black  |
| cat    | 18lb   | calico |
```


## Note：
如果Excel表格中有换行符，可批量替换Ctrl+J，为空格，可批量消除Excel表格中的换行符。

在查找内容框内点击后，按组合键Ctrl+J (注意不是输入)，点击“全部替换”；即可清除所有换行符。
