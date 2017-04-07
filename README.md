# api documentation for  [shipit-cli (v3.0.0)](https://github.com/shipitjs/shipit)  [![npm package](https://img.shields.io/npm/v/npmdoc-shipit-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-shipit-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-shipit-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-shipit-cli)
#### Universal automation and deployment tool written in JavaScript.

[![NPM](https://nodei.co/npm/shipit-cli.png?downloads=true)](https://www.npmjs.com/package/shipit-cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-shipit-cli/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-shipit-cli_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-shipit-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-shipit-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-shipit-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Greg Bergé",
        "email": "berge.greg@gmail.com"
    },
    "bin": {
        "shipit": "./bin/shipit"
    },
    "bugs": {
        "url": "https://github.com/shipitjs/shipit/issues"
    },
    "dependencies": {
        "bluebird": "^3.3.4",
        "chalk": "^1.0.0",
        "interpret": "^1.0.0",
        "liftoff": "^2.0.0",
        "lodash": "^4.6.1",
        "minimist": "^1.1.0",
        "orchestrator": "^0.3.7",
        "pretty-hrtime": "^1.0.0",
        "ssh-pool": "^1.0.0",
        "stream-line-wrapper": "^0.1.1",
        "v8flags": "^2.0.2"
    },
    "description": "Universal automation and deployment tool written in JavaScript.",
    "devDependencies": {
        "chai": "^3.0.0",
        "mocha": "^2.1.0",
        "mock-utf8-stream": "^0.1.1",
        "sinon": "^1.12.2",
        "sinon-chai": "^2.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a9ad1185146ddc80951a8eb6b762d9e8b6587cba",
        "tarball": "https://registry.npmjs.org/shipit-cli/-/shipit-cli-3.0.0.tgz"
    },
    "gitHead": "bdff0ccea49cf762942c4124ecefea1300fad885",
    "homepage": "https://github.com/shipitjs/shipit",
    "keywords": [
        "shipit",
        "automation",
        "deployment",
        "deploy",
        "ssh"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "neoziro",
            "email": "berge.greg@gmail.com"
        },
        {
            "name": "timkelty",
            "email": "tim@fusionary.com"
        }
    ],
    "name": "shipit-cli",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/shipitjs/shipit.git"
    },
    "scripts": {
        "test": "mocha && ./bin/shipit staging test"
    },
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module shipit-cli](#apidoc.module.shipit-cli)
1.  [function <span class="apidocSignatureSpan">shipit-cli.</span>super_ ()](#apidoc.element.shipit-cli.super_)
1.  object <span class="apidocSignatureSpan">shipit-cli.</span>super_.prototype

#### [module shipit-cli.super_](#apidoc.module.shipit-cli.super_)
1.  [function <span class="apidocSignatureSpan">shipit-cli.</span>super_ ()](#apidoc.element.shipit-cli.super_.super_)

#### [module shipit-cli.super_.prototype](#apidoc.module.shipit-cli.super_.prototype)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_emitTaskDone (task, message, err)](#apidoc.element.shipit-cli.super_.prototype._emitTaskDone)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_readyToRunTask (task)](#apidoc.element.shipit-cli.super_.prototype._readyToRunTask)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetAllTasks ()](#apidoc.element.shipit-cli.super_.prototype._resetAllTasks)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetSpecificTasks (names)](#apidoc.element.shipit-cli.super_.prototype._resetSpecificTasks)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetTask (task)](#apidoc.element.shipit-cli.super_.prototype._resetTask)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_runStep ()](#apidoc.element.shipit-cli.super_.prototype._runStep)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_runTask (task)](#apidoc.element.shipit-cli.super_.prototype._runTask)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_stopTask (task, meta)](#apidoc.element.shipit-cli.super_.prototype._stopTask)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>add (name, dep, fn)](#apidoc.element.shipit-cli.super_.prototype.add)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>allDone ()](#apidoc.element.shipit-cli.super_.prototype.allDone)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>hasTask (name)](#apidoc.element.shipit-cli.super_.prototype.hasTask)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>onAll (callback)](#apidoc.element.shipit-cli.super_.prototype.onAll)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>reset ()](#apidoc.element.shipit-cli.super_.prototype.reset)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>sequence (tasks, names, results, nest)](#apidoc.element.shipit-cli.super_.prototype.sequence)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>start ()](#apidoc.element.shipit-cli.super_.prototype.start)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>stop (err, successfulFinish)](#apidoc.element.shipit-cli.super_.prototype.stop)
1.  [function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>task (name, dep, fn)](#apidoc.element.shipit-cli.super_.prototype.task)



# <a name="apidoc.module.shipit-cli"></a>[module shipit-cli](#apidoc.module.shipit-cli)

#### <a name="apidoc.element.shipit-cli.super_"></a>[function <span class="apidocSignatureSpan">shipit-cli.</span>super_ ()](#apidoc.element.shipit-cli.super_)
- description and source-code
```javascript
super_ = function () {
	EventEmitter.call(this);
	this.doneCallback = undefined; // call this when all tasks in the queue are done
	this.seq = []; // the order to run the tasks
	this.tasks = {}; // task objects: name, dep (list of names of dependencies), fn (the task to run)
	this.isRunning = false; // is the orchestrator running tasks? .start() to start, .stop() to stop
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit-cli.super_"></a>[module shipit-cli.super_](#apidoc.module.shipit-cli.super_)

#### <a name="apidoc.element.shipit-cli.super_.super_"></a>[function <span class="apidocSignatureSpan">shipit-cli.</span>super_ ()](#apidoc.element.shipit-cli.super_.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit-cli.super_.prototype"></a>[module shipit-cli.super_.prototype](#apidoc.module.shipit-cli.super_.prototype)

#### <a name="apidoc.element.shipit-cli.super_.prototype._emitTaskDone"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_emitTaskDone (task, message, err)](#apidoc.element.shipit-cli.super_.prototype._emitTaskDone)
- description and source-code
```javascript
_emitTaskDone = function (task, message, err) {
		if (!task.args) {
			task.args = {task:task.name};
		}
		task.args.duration = task.duration;
		task.args.hrDuration = task.hrDuration;
		task.args.message = task.name+' '+message;
		var evt = 'stop';
		if (err) {
			task.args.err = err;
			evt = 'err';
		}
		// 'task_stop' or 'task_err'
		this.emit('task_'+evt, task.args);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._readyToRunTask"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_readyToRunTask (task)](#apidoc.element.shipit-cli.super_.prototype._readyToRunTask)
- description and source-code
```javascript
_readyToRunTask = function (task) {
		var ready = true, // no one disproved it yet
			i, name, t;
		if (task.dep.length) {
			for (i = 0; i < task.dep.length; i++) {
				name = task.dep[i];
				t = this.tasks[name];
				if (!t) {
					// FRAGILE: this should never happen
					this.stop("can't run "+task.name+" because it depends on "+name+" which doesn't exist");
					ready = false;
					break;
				}
				if (!t.done) {
					ready = false;
					break;
				}
			}
		}
		return ready;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._resetAllTasks"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetAllTasks ()](#apidoc.element.shipit-cli.super_.prototype._resetAllTasks)
- description and source-code
```javascript
_resetAllTasks = function () {
		var task;
		for (task in this.tasks) {
			if (this.tasks.hasOwnProperty(task)) {
				this._resetTask(this.tasks[task]);
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._resetSpecificTasks"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetSpecificTasks (names)](#apidoc.element.shipit-cli.super_.prototype._resetSpecificTasks)
- description and source-code
```javascript
_resetSpecificTasks = function (names) {
		var i, name, t;

		if (names && names.length) {
			for (i = 0; i < names.length; i++) {
				name = names[i];
				t = this.tasks[name];
				if (t) {
					this._resetTask(t);
					if (t.dep && t.dep.length) {
						this._resetSpecificTasks(t.dep); // recurse
					}
				//} else {
					// FRAGILE: ignore that the task doesn't exist
				}
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._resetTask"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_resetTask (task)](#apidoc.element.shipit-cli.super_.prototype._resetTask)
- description and source-code
```javascript
_resetTask = function (task) {
		if (task) {
			if (task.done) {
				task.done = false;
			}
			delete task.start;
			delete task.stop;
			delete task.duration;
			delete task.hrDuration;
			delete task.args;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._runStep"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_runStep ()](#apidoc.element.shipit-cli.super_.prototype._runStep)
- description and source-code
```javascript
_runStep = function () {
		var i, task;
		if (!this.isRunning) {
			return; // user aborted, ASSUME: stop called previously
		}
		for (i = 0; i < this.seq.length; i++) {
			task = this.tasks[this.seq[i]];
			if (!task.done && !task.running && this._readyToRunTask(task)) {
				this._runTask(task);
			}
			if (!this.isRunning) {
				return; // task failed or user aborted, ASSUME: stop called previously
			}
		}
		if (this.allDone()) {
			this.stop(null, true);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._runTask"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_runTask (task)](#apidoc.element.shipit-cli.super_.prototype._runTask)
- description and source-code
```javascript
_runTask = function (task) {
		var that = this;

		task.args = {task:task.name, message:task.name+' started'};
		this.emit('task_start', task.args);
		task.running = true;

		runTask(task.fn.bind(this), function (err, meta) {
			that._stopTask.call(that, task, meta);
			that._emitTaskDone.call(that, task, meta.runMethod, err);
			if (err) {
				return that.stop.call(that, err);
			}
			that._runStep.call(that);
		});
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype._stopTask"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>_stopTask (task, meta)](#apidoc.element.shipit-cli.super_.prototype._stopTask)
- description and source-code
```javascript
_stopTask = function (task, meta) {
		task.duration = meta.duration;
		task.hrDuration = meta.hrDuration;
		task.running = false;
		task.done = true;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.add"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>add (name, dep, fn)](#apidoc.element.shipit-cli.super_.prototype.add)
- description and source-code
```javascript
add = function (name, dep, fn) {
		if (!fn && typeof dep === 'function') {
			fn = dep;
			dep = undefined;
		}
		dep = dep || [];
		fn = fn || function () {}; // no-op
		if (!name) {
			throw new Error('Task requires a name');
		}
		// validate name is a string, dep is an array of strings, and fn is a function
		if (typeof name !== 'string') {
			throw new Error('Task requires a name that is a string');
		}
		if (typeof fn !== 'function') {
			throw new Error('Task '+name+' requires a function that is a function');
		}
		if (!Array.isArray(dep)) {
			throw new Error('Task '+name+' can\'t support dependencies that is not an array of strings');
		}
		dep.forEach(function (item) {
			if (typeof item !== 'string') {
				throw new Error('Task '+name+' dependency '+item+' is not a string');
			}
		});
		this.tasks[name] = {
			fn: fn,
			dep: dep,
			name: name
		};
		return this;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.allDone"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>allDone ()](#apidoc.element.shipit-cli.super_.prototype.allDone)
- description and source-code
```javascript
allDone = function () {
		var i, task, allDone = true; // nothing disputed it yet
		for (i = 0; i < this.seq.length; i++) {
			task = this.tasks[this.seq[i]];
			if (!task.done) {
				allDone = false;
				break;
			}
		}
		return allDone;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.hasTask"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>hasTask (name)](#apidoc.element.shipit-cli.super_.prototype.hasTask)
- description and source-code
```javascript
hasTask = function (name) {
		return !!this.tasks[name];
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.onAll"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>onAll (callback)](#apidoc.element.shipit-cli.super_.prototype.onAll)
- description and source-code
```javascript
onAll = function (callback) {
		var i;
		if (typeof callback !== 'function') {
			throw new Error('No callback specified');
		}

		for (i = 0; i < events.length; i++) {
			listenToEvent(this, events[i], callback);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.reset"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>reset ()](#apidoc.element.shipit-cli.super_.prototype.reset)
- description and source-code
```javascript
reset = function () {
		if (this.isRunning) {
			this.stop(null);
		}
		this.tasks = {};
		this.seq = [];
		this.isRunning = false;
		this.doneCallback = undefined;
		return this;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.sequence"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>sequence (tasks, names, results, nest)](#apidoc.element.shipit-cli.super_.prototype.sequence)
- description and source-code
```javascript
sequence = function (tasks, names, results, nest) {
	var i, name, node, e, j;
	nest = nest || [];
	for (i = 0; i < names.length; i++) {
		name = names[i];
		// de-dup results
		if (results.indexOf(name) === -1) {
			node = tasks[name];
			if (!node) {
				e = new Error('task "'+name+'" is not defined');
				e.missingTask = name;
				e.taskList = [];
				for (j in tasks) {
					if (tasks.hasOwnProperty(j)) {
						e.taskList.push(tasks[j].name);
					}
				}
				throw e;
			}
			if (nest.indexOf(name) > -1) {
				nest.push(name);
				e = new Error('Recursive dependencies detected: '+nest.join(' -> '));
				e.recursiveTasks = nest;
				e.taskList = [];
				for (j in tasks) {
					if (tasks.hasOwnProperty(j)) {
						e.taskList.push(tasks[j].name);
					}
				}
				throw e;
			}
			if (node.dep.length) {
				nest.push(name);
				sequence(tasks, node.dep, results, nest); // recurse
				nest.pop(name);
			}
			results.push(name);
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.start"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>start ()](#apidoc.element.shipit-cli.super_.prototype.start)
- description and source-code
```javascript
start = function () {
		var args, arg, names = [], lastTask, i, seq = [];
		args = Array.prototype.slice.call(arguments, 0);
		if (args.length) {
			lastTask = args[args.length-1];
			if (typeof lastTask === 'function') {
				this.doneCallback = lastTask;
				args.pop();
			}
			for (i = 0; i < args.length; i++) {
				arg = args[i];
				if (typeof arg === 'string') {
					names.push(arg);
				} else if (Array.isArray(arg)) {
					names = names.concat(arg); // FRAGILE: ASSUME: it's an array of strings
				} else {
					throw new Error('pass strings or arrays of strings');
				}
			}
		}
		if (this.isRunning) {
			// reset specified tasks (and dependencies) as not run
			this._resetSpecificTasks(names);
		} else {
			// reset all tasks as not run
			this._resetAllTasks();
		}
		if (this.isRunning) {
			// if you call start() again while a previous run is still in play
			// prepend the new tasks to the existing task queue
			names = names.concat(this.seq);
		}
		if (names.length < 1) {
			// run all tasks
			for (i in this.tasks) {
				if (this.tasks.hasOwnProperty(i)) {
					names.push(this.tasks[i].name);
				}
			}
		}
		seq = [];
		try {
			this.sequence(this.tasks, names, seq, []);
		} catch (err) {
			// Is this a known error?
			if (err) {
				if (err.missingTask) {
					this.emit('task_not_found', {message: err.message, task:err.missingTask, err: err});
				}
				if (err.recursiveTasks) {
					this.emit('task_recursion', {message: err.message, recursiveTasks:err.recursiveTasks, err: err});
				}
			}
			this.stop(err);
			return this;
		}
		this.seq = seq;
		this.emit('start', {message:'seq: '+this.seq.join(',')});
		if (!this.isRunning) {
			this.isRunning = true;
		}
		this._runStep();
		return this;
	}
```
- example usage
```shell
...
'''js
shipit.task('build', function () {
  // ...
  shipit.emit('built');
});

shipit.on('built', function () {
  shipit.start('start-server');
});
'''

Shipit emits the 'init' event once initialized, before any tasks are run.

### Methods
...
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.stop"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>stop (err, successfulFinish)](#apidoc.element.shipit-cli.super_.prototype.stop)
- description and source-code
```javascript
stop = function (err, successfulFinish) {
		this.isRunning = false;
		if (err) {
			this.emit('err', {message:'orchestration failed', err:err});
		} else if (successfulFinish) {
			this.emit('stop', {message:'orchestration succeeded'});
		} else {
			// ASSUME
			err = 'orchestration aborted';
			this.emit('err', {message:'orchestration aborted', err: err});
		}
		if (this.doneCallback) {
			// Avoid calling it multiple times
			this.doneCallback(err);
		} else if (err && !this.listeners('err').length) {
			// No one is listening for the error so speak louder
			throw err;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit-cli.super_.prototype.task"></a>[function <span class="apidocSignatureSpan">shipit-cli.super_.prototype.</span>task (name, dep, fn)](#apidoc.element.shipit-cli.super_.prototype.task)
- description and source-code
```javascript
task = function (name, dep, fn) {
		if (dep || fn) {
			// alias for add, return nothing rather than this
			this.add(name, dep, fn);
		} else {
			return this.tasks[name];
		}
	}
```
- example usage
```shell
...
module.exports = function (shipit) {
  shipit.initConfig({
    staging: {
      servers: 'myproject.com'
    }
  });

  shipit.task('pwd', function () {
    return shipit.remote('pwd');
  });
};
'''

### Launch command
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
