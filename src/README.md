This is a plugin that adds a type of selection for focusing places
that don't allow regular selection (such as positions that have a leaf
block node, table, or the end of the document both before and after
them).

@cn 本插件为那些不允许正常选区的聚焦的位置（比如说该位置有叶子节点、表格、或者文档的起始和结尾处）添加一种选区的类型。

You'll probably want to load `style/gapcursor.css`, which contains
basic styling for the simulated cursor (as a short, blinking
horizontal stripe).

@cn 你可能需要加载 `style/gapcursor.css` 这个文件，它包含了模拟光标的基本样式（即短的，闪烁的水平条纹）。

By default, gap cursor are only allowed in places where the default
content node (in the schema content constraints) is a textblock node.
You can customize this by adding an `allowGapCursor` property to your
node specs—if it's true, gap cursor are allowed everywhere in that
node, if it's `false` they are never allowed.

@cn 默认情况下，gap 光标只允许放置于默认内容节点（通过 schema 的 content 限制）是文本节点的地方。你可以通过在节点配置对象中添加
`allowGapCursor` 属性来自定义这个行为，如果该值是 true，则 gap 光标被允许放置到该节点的任何位置，如果是 `false` 则表示永远不允许放置该种类型的光标。

@gapCursor

@GapCursor
