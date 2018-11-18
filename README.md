# Annotate Kubernetes

Kubernetes 版本 release-1.13

```
git clone git@github.com:lizebang/annotate-kubernetes.git $GOPATH/src/k8s.io/kubernetes
```

## Prepare

我使用的是 vscode，你们也可以使用它，同时推荐安装 [Go](https://marketplace.visualstudio.com/items?itemName=ms-vscode.Go)、[todo-highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight) 和 [todo-tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree) 这三个插件。

## Settings

我的 `todo-highlight` 和 `todo-tree` 设置如下：

```settings
	// todohighlight
	"todohighlight.keywords": [
		{
			"text": "TODO:",
			"color": "#000",
			"backgroundColor": "#ffbd2a",
			"overviewRulerColor": "rgba(255,189,42,0.8)"
		},
		{
			"text": "FIXME:",
			"color": "#000",
			"backgroundColor": "#f06292",
			"overviewRulerColor": "rgba(240,98,146,0.8)"
		},
		{
			"text": "NOTE:",
			"color": "#000",
			"backgroundColor": "#00F0F0",
			"overviewRulerColor": "rgba(240,98,146,0.8)"
		},
		{
			"text": "TS:",
			"color": "#000",
			"backgroundColor": "#aa00aa",
			"overviewRulerColor": "rgba(240,98,146,0.8)"
		},
		{
			"text": "IMP:",
			"color": "#000",
			"backgroundColor": "#a287f4",
			"overviewRulerColor": "rgba(240,98,146,0.8)"
		},
		{
			"text": "TSK:",
			"color": "#000",
			"backgroundColor": "#00aaFF",
			"overviewRulerColor": "rgba(240,98,146,0.8)"
		}
	],

	// todo-tree
	"todo-tree.defaultHighlight": {
		"foreground": "green",
		"background": "white",
		"type": "none"
	},
	"todo-tree.tags": ["TODO:", "FIXME:", "NOTE:", "TS:", "IMP:", "TSK:"],
	"todo-tree.customHighlight": {
		"TODO:": {},
		"FIXME:": {},
		"NOTE:": {},
		"TS:": {},
		"IMP:": {},
		"TSK:": {}
	},
```

`TS:`、`IMP:`、`TSK:` 是我自己定义的，它们的含义是：

- `TS:` translate 翻译
- `IMP:` important 重要
- `TSK:` task 任务
