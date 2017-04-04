# api documentation for  [vows (v0.8.1)](https://github.com/cloudhead/vows)  [![npm package](https://img.shields.io/npm/v/npmdoc-vows.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vows) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vows.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vows)
#### Asynchronous BDD & continuous integration for node.js

[![NPM](https://nodei.co/npm/vows.png?downloads=true)](https://www.npmjs.com/package/vows)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vows/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vows_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vows/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vows/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vows/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alexis Sellier",
        "email": "self@cloudhead.net"
    },
    "bin": {
        "vows": "./bin/vows"
    },
    "bugs": {
        "url": "https://github.com/cloudhead/vows/issues"
    },
    "contributors": [
        {
            "name": "Charlie Robbins",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "Jerry Sievert",
            "email": "jerry@legitimatesounding.com"
        }
    ],
    "dependencies": {
        "diff": "~1.0.8",
        "eyes": "~0.1.6",
        "glob": "~4.0.6"
    },
    "description": "Asynchronous BDD & continuous integration for node.js",
    "devDependencies": {},
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "e09e988ce594ca05a08d72abcca34e88db559131",
        "tarball": "https://registry.npmjs.org/vows/-/vows-0.8.1.tgz"
    },
    "gitHead": "81333f31df9ea7a64896d0f9415077a1bc500869",
    "homepage": "https://github.com/cloudhead/vows",
    "keywords": [
        "testing",
        "spec",
        "test",
        "BDD"
    ],
    "license": "MIT",
    "main": "./lib/vows",
    "maintainers": [
        {
            "name": "cloudhead",
            "email": "self@cloudhead.net"
        },
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "mmalecki",
            "email": "maciej.malecki@notimplemented.org"
        },
        {
            "name": "jerrysievert",
            "email": "code@legitimatesounding.com"
        }
    ],
    "name": "vows",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cloudhead/vows.git"
    },
    "scripts": {
        "test": "node ./bin/vows --spec"
    },
    "url": "http://vowsjs.org",
    "version": "0.8.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vows](#apidoc.module.vows)
1.  [function <span class="apidocSignatureSpan">vows.</span>describe (subject)](#apidoc.element.vows.describe)
1.  [function <span class="apidocSignatureSpan">vows.</span>inspect (val)](#apidoc.element.vows.inspect)
1.  [function <span class="apidocSignatureSpan">vows.</span>prepare (obj, targets)](#apidoc.element.vows.prepare)
1.  [function <span class="apidocSignatureSpan">vows.</span>tryEnd (batch)](#apidoc.element.vows.tryEnd)
1.  object <span class="apidocSignatureSpan">vows.</span>console
1.  object <span class="apidocSignatureSpan">vows.</span>options
1.  object <span class="apidocSignatureSpan">vows.</span>reporter
1.  object <span class="apidocSignatureSpan">vows.</span>suites
1.  string <span class="apidocSignatureSpan">vows.</span>version

#### [module vows.console](#apidoc.module.vows.console)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>contextText (event)](#apidoc.element.vows.console.contextText)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>error (obj)](#apidoc.element.vows.console.error)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>inspect (val)](#apidoc.element.vows.console.inspect)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>log (args)](#apidoc.element.vows.console.log)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>puts (options)](#apidoc.element.vows.console.puts)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>result (event)](#apidoc.element.vows.console.result)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>stylize (str, style)](#apidoc.element.vows.console.stylize)
1.  [function <span class="apidocSignatureSpan">vows.console.</span>vowText (event)](#apidoc.element.vows.console.vowText)

#### [module vows.options](#apidoc.module.vows.options)
1.  boolean <span class="apidocSignatureSpan">vows.options.</span>error
1.  [function <span class="apidocSignatureSpan">vows.options.</span>Emitter ()](#apidoc.element.vows.options.Emitter)
1.  object <span class="apidocSignatureSpan">vows.options.</span>matcher
1.  object <span class="apidocSignatureSpan">vows.options.</span>reporter

#### [module vows.reporter](#apidoc.module.vows.reporter)
1.  [function <span class="apidocSignatureSpan">vows.reporter.</span>print (str)](#apidoc.element.vows.reporter.print)
1.  [function <span class="apidocSignatureSpan">vows.reporter.</span>report (data)](#apidoc.element.vows.reporter.report)
1.  [function <span class="apidocSignatureSpan">vows.reporter.</span>reset ()](#apidoc.element.vows.reporter.reset)
1.  [function <span class="apidocSignatureSpan">vows.reporter.</span>setStream (s)](#apidoc.element.vows.reporter.setStream)
1.  string <span class="apidocSignatureSpan">vows.reporter.</span>name



# <a name="apidoc.module.vows"></a>[module vows](#apidoc.module.vows)

#### <a name="apidoc.element.vows.describe"></a>[function <span class="apidocSignatureSpan">vows.</span>describe (subject)](#apidoc.element.vows.describe)
- description and source-code
```javascript
describe = function (subject) {
    var suite = new(Suite)(subject);

    this.options.Emitter.prototype.addVow = addVow;
    // just in case someone emit's before I get to it
    this.options.Emitter.prototype.emit = function (event) {
        this._vowsEmitedEvents = this._vowsEmitedEvents || {};
        this._vowsEmitedEventsOrder = this._vowsEmitedEventsOrder || [];
        // slice off the event
        var args = Array.prototype.slice.call(arguments, 1);
        // if multiple events are fired, add or push
        if (this._vowsEmitedEvents.hasOwnProperty(event)) {
            this._vowsEmitedEvents[event].push(args);
        } else {
            this._vowsEmitedEvents[event] = [args];
        }

        // push the event onto a stack so I have an order
        this._vowsEmitedEventsOrder.push(event);
        return oldEmit.apply(this, arguments);
    }
    this.suites.push(suite);

    //
    // Add any additional arguments as batches if they're present
    //
    if (arguments.length > 1) {
        for (var i = 1, l = arguments.length; i < l; ++i) {
            suite.addBatch(arguments[i]);
        }
    }

    return suite;
}
```
- example usage
```shell
...
synopsis
--------

'''js
var vows = require('vows'),
assert = require('assert');

vows.describe('Deep Thought').addBatch({
'An instance of DeepThought': {
    topic: new DeepThought,

    'should know the answer to the ultimate question of life': function (deepThought) {
        assert.equal (deepThought.question('what is the answer to the universe?'), 42);
    }
}
...
```

#### <a name="apidoc.element.vows.inspect"></a>[function <span class="apidocSignatureSpan">vows.</span>inspect (val)](#apidoc.element.vows.inspect)
- description and source-code
```javascript
function inspect(val) {
    if (module.exports.nocolor) {
      return eyes(val);
    }

    return '\033[1m' + eyes(val) + '\033[22m';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.prepare"></a>[function <span class="apidocSignatureSpan">vows.</span>prepare (obj, targets)](#apidoc.element.vows.prepare)
- description and source-code
```javascript
prepare = function (obj, targets) {
    targets.forEach(function (target) {
        if (target in obj) {
            obj[target] = (function (fun) {
                return function () {
                    var args = Array.prototype.slice.call(arguments);
                    var ee = new(events.EventEmitter);

                    args.push(function (err /* [, data] */) {
                        var args = Array.prototype.slice.call(arguments, 1);

                        if (err) { ee.emit.apply(ee, ['error', err].concat(args)) }
                        else     { ee.emit.apply(ee, ['success'].concat(args)) }
                    });
                    fun.apply(obj, args);

                    return ee;
                };
            })(obj[target]);
        }
    });
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.tryEnd"></a>[function <span class="apidocSignatureSpan">vows.</span>tryEnd (batch)](#apidoc.element.vows.tryEnd)
- description and source-code
```javascript
tryEnd = function (batch) {
    var result, style, time;

    if (batch.honored + batch.broken + batch.errored + batch.pending === batch.total &&
        batch.remaining === 0) {

        Object.keys(batch).forEach(function (k) {
            (k in batch.suite.results) && (batch.suite.results[k] += batch[k]);
        });

        if (batch.teardowns) {
            for (var i = batch.teardowns.length - 1, ctx; i >= 0; i--) {
                runTeardown(batch.teardowns[i]);
            }

            maybeFinish();
        }

        function runTeardown(teardown) {
            var env = Object.create(teardown.env);

            Object.defineProperty(env, "callback", {
                get: function () {
                    teardown.awaitingCallback = true;

                    return function () {
                        teardown.awaitingCallback = false;
                        maybeFinish();
                    };
                }
            });

            teardown.tests.teardown.apply(env, teardown.topics);
        }

        function maybeFinish() {
            var pending = batch.teardowns.filter(function (teardown) {
                return teardown.awaitingCallback;
            });

            if (pending.length === 0) {
                finish();
            }
        }

        function finish() {
            batch.status = 'end';
            batch.suite.report(['end']);
            batch.emitter.emit('end', batch.honored, batch.broken, batch.errored, batch.pending);
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vows.console"></a>[module vows.console](#apidoc.module.vows.console)

#### <a name="apidoc.element.vows.console.contextText"></a>[function <span class="apidocSignatureSpan">vows.console.</span>contextText (event)](#apidoc.element.vows.console.contextText)
- description and source-code
```javascript
contextText = function (event) {
    return '  ' + event;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.error"></a>[function <span class="apidocSignatureSpan">vows.console.</span>error (obj)](#apidoc.element.vows.console.error)
- description and source-code
```javascript
error = function (obj) {
    var string  = '✗ ' + $('Errored ').red + '» ';
        string += $(obj.error).red.bold                         + '\n';
        string += (obj.context ? '    in ' + $(obj.context).red + '\n': '');
        string += '    in ' + $(obj.suite.subject).red          + '\n';
        string += '    in ' + $(obj.suite._filename).red;

    return string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.inspect"></a>[function <span class="apidocSignatureSpan">vows.console.</span>inspect (val)](#apidoc.element.vows.console.inspect)
- description and source-code
```javascript
function inspect(val) {
    if (module.exports.nocolor) {
      return eyes(val);
    }

    return '\033[1m' + eyes(val) + '\033[22m';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.log"></a>[function <span class="apidocSignatureSpan">vows.console.</span>log (args)](#apidoc.element.vows.console.log)
- description and source-code
```javascript
log = function (args) {
    args = Array.prototype.slice.call(arguments);
    if (!options.raw) {
        args = args.map(function (a) {
            return a.replace(/'([^']+)'/g,   function (_, capture) { return stylize(capture, 'italic') })
                    .replace(/\*([^*]+)\*/g, function (_, capture) { return stylize(capture, 'bold') })
                    .replace(/\n/g, function (_, capture) { return ' \n  ' } );
        });
    }
    return options.stream.write(args.join('\n') + options.tail);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.puts"></a>[function <span class="apidocSignatureSpan">vows.console.</span>puts (options)](#apidoc.element.vows.console.puts)
- description and source-code
```javascript
puts = function (options) {
    var stylize = exports.stylize;
    options.stream || (options.stream = process.stdout);
    options.tail = options.tail || '';

    return function (args) {
        args = Array.prototype.slice.call(arguments);
        if (!options.raw) {
            args = args.map(function (a) {
                return a.replace(/'([^']+)'/g,   function (_, capture) { return stylize(capture, 'italic') })
                        .replace(/\*([^*]+)\*/g, function (_, capture) { return stylize(capture, 'bold') })
                        .replace(/\n/g, function (_, capture) { return ' \n  ' } );
            });
        }
        return options.stream.write(args.join('\n') + options.tail);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.result"></a>[function <span class="apidocSignatureSpan">vows.console.</span>result (event)](#apidoc.element.vows.console.result)
- description and source-code
```javascript
result = function (event) {
    var result = [], buffer = [], time = '', header;
    var complete = event.honored + event.pending + event.errored + event.broken;
    var status = (event.errored && 'errored') || (event.broken && 'broken') ||
                 (event.honored && 'honored') || (event.pending && 'pending');

    if (event.total === 0) {
        return [$("Could not find any tests to run.").bold.red];
    }

    event.honored && result.push($(event.honored).bold + " honored");
    event.broken  && result.push($(event.broken).bold  + " broken");
    event.errored && result.push($(event.errored).bold + " errored");
    event.pending && result.push($(event.pending).bold + " pending");

    if (complete < event.total) {
        result.push($(event.total - complete).bold + " dropped");
    }

    result = result.join(' ∙ ');

    header = {
        honored: '✓ ' + $('OK').bold.green,
        broken:  '✗ ' + $('Broken').bold.yellow,
        errored: '✗ ' + $('Errored').bold.red,
        pending: '- ' + $('Pending').bold.cyan
    }[status] + ' » ';

    if (typeof(event.time) === 'number') {
        time = ' (' + event.time.toFixed(3) + 's)';
        time = this.stylize(time, 'grey');
    }
    buffer.push(header + result + time + '\n');

    return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.stylize"></a>[function <span class="apidocSignatureSpan">vows.console.</span>stylize (str, style)](#apidoc.element.vows.console.stylize)
- description and source-code
```javascript
function stylize(str, style) {
    if (module.exports.nocolor) {
      return str;
    }

    var styles = {
        'bold'      : [1,  22],
        'italic'    : [3,  23],
        'underline' : [4,  24],
        'cyan'      : [96, 39],
        'yellow'    : [33, 39],
        'green'     : [32, 39],
        'red'       : [31, 39],
        'grey'      : [90, 39],
        'green-hi'  : [92, 32],
    };
    return '\033[' + styles[style][0] + 'm' + str +
           '\033[' + styles[style][1] + 'm';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.console.vowText"></a>[function <span class="apidocSignatureSpan">vows.console.</span>vowText (event)](#apidoc.element.vows.console.vowText)
- description and source-code
```javascript
vowText = function (event) {
    var buffer = [];

    buffer.push('   ' + {
        honored: ' ✓ ',
        broken:  ' ✗ ',
        errored: ' ✗ ',
        pending: ' - '
    }[event.status] + this.stylize(event.title, ({
        honored: 'green',
        broken:  'yellow',
        errored: 'red',
        pending: 'cyan'
    })[event.status]));

    if (event.status === 'broken') {
        buffer.push('      » ' + event.exception);
    } else if (event.status === 'errored') {
        if (event.exception.type === 'emitter') {
            buffer.push('      » ' + this.stylize("An unexpected error was caught: " +
                           this.stylize(event.exception.error, 'bold'), 'red'));
        } else {
            buffer.push('    ' + this.stylize(event.exception, 'red'));
        }
    }
    return buffer.join('\n');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vows.options"></a>[module vows.options](#apidoc.module.vows.options)

#### <a name="apidoc.element.vows.options.Emitter"></a>[function <span class="apidocSignatureSpan">vows.options.</span>Emitter ()](#apidoc.element.vows.options.Emitter)
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



# <a name="apidoc.module.vows.reporter"></a>[module vows.reporter](#apidoc.module.vows.reporter)

#### <a name="apidoc.element.vows.reporter.print"></a>[function <span class="apidocSignatureSpan">vows.reporter.</span>print (str)](#apidoc.element.vows.reporter.print)
- description and source-code
```javascript
print = function (str) {
    puts(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.reporter.report"></a>[function <span class="apidocSignatureSpan">vows.reporter.</span>report (data)](#apidoc.element.vows.reporter.report)
- description and source-code
```javascript
report = function (data) {
    var event = data[1];

    switch (data[0]) {
        case 'subject':
            // messages.push(stylize(event, 'underline') + '\n');
            break;
        case 'context':
            break;
        case 'vow':
            if (event.status === 'honored') {
                puts(stylize('·', 'green'));
            } else if (event.status === 'pending') {
                puts(stylize('-', 'cyan'));
            } else {
                if (lastContext !== event.context) {
                    lastContext = event.context;
                    messages.push('  ' + event.context);
                }
                if (event.status === 'broken') {
                    puts(stylize('✗', 'yellow'));
                    messages.push(console.vowText(event));
                } else if (event.status === 'errored') {
                    puts(stylize('✗', 'red'));
                    messages.push(console.vowText(event));
                }
                messages.push('');
            }
            break;
        case 'end':
            puts(' ');
            break;
        case 'finish':
            if (messages.length) {
                puts('\n\n' + messages.join('\n'));
            } else {
                puts('');
            }
            puts(console.result(event).join('\n'));
            break;
        case 'error':
            puts(console.error(event));
            break;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.reporter.reset"></a>[function <span class="apidocSignatureSpan">vows.reporter.</span>reset ()](#apidoc.element.vows.reporter.reset)
- description and source-code
```javascript
reset = function () {
    messages = [];
    lastContext = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vows.reporter.setStream"></a>[function <span class="apidocSignatureSpan">vows.reporter.</span>setStream (s)](#apidoc.element.vows.reporter.setStream)
- description and source-code
```javascript
setStream = function (s) {
    options.stream = s;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
