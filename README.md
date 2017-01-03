# mmTrix Agent for Node.js

[![NPM](https://nodei.co/npm/mmtrix.png?downloads=true&stars=true)](https://nodei.co/npm/mmtrix/)
[![NPM](https://nodei.co/npm-dl/mmtrix.png?months=6)](https://nodei.co/npm/mmtrix/)

## 使用方法
1. 安装mmtrix angent

	```bash
		cd /你的项目目录
		npm i mmtrix --save
	```

2. 拷贝配置文件到项目根目录

	```bash
		cp ./node_modules/mmtrix/mmtrix.js .
	```

3. 修改配置文件

	```
		打开./mmtrix.js 修改项目名称和licenseKey
	```
4. 开始使用

	在你的项目主文件的第一行添加代码：

	```javascript
		require('mmtrix');
	```

5. 运行你的应用，等待5分钟后可以到mmtrix管理页面查看应用的运行数据。


	## DEMO
	```javascript
		var mmtrix = require('mmtrix');
		var app = require('express')();
		app.locals.mmtrix = mmtrix;
		app.get('/user/:id', function (req, res) {
			res.render('user');
		});
		app.listen(process.env.PORT);
	```
