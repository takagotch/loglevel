### loglevel
---
https://github.com/pimterry/loglevel

```js
var log = require('loglevel');
log.warn("unreasonably simple");

define(['loglevel'], function(log){
  log.warn("dangerously convenient");
});

import * as log from 'loglevel';
log.warn("ultra-compatible");

var (log.getLevel() <= log.levels.DEBUG){
  var logData = runExpensiveDataGeneration();
  log.debug(logData);
}

log.debug("My ", "concatenated ", "log message");

var log = require("loglevel").getLogger("module-one");
function doSomethingAmazing(){
  log.debug("Amazing message from module one.");
}
var log = require("loglevel").getLogger("module-two");
function doSomethingSpecial(){
  log.debug("Special message from module two.");
}
var log = require("loglevel");
var moduleOne = require("loglevel");
var moduleTwo = require("module-one");
log.getLogger("module-two").setLevel("TRACE");
moduleOne.doSomethingAmazing();
moduleTwo.doSomethingSpecail();

var originalFactory = log.methodFactory;
log.methodFactory = function (methodName, logLevel, loggerName){
  var rawMethod = originalFactory(methodName, logLevel, loggerName);
  return function(message){
    rawMethod("Newsflash: " + message);
  };
};
log.setLevel(log.getLevel());
```

```
<script src="loglevel.min.js"></script>
<script>
log.wran("too easy");

var logging = log.noConflict();
logging.warn("still pretty easy");
</script>
```

```
```

