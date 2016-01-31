# Angular2Sample

Anqular2 Sample

Initially based on Angular's 5 Min Quickstart sample: https://angular.io/docs/ts/latest/quickstart.html#

server-lite process would crash every time.
First, only error at EventEmitter.emit at event.js was visible.
After first two changes from the list below spawn cmd ENOENT error appeared.
The third change is probably the original problem solver.
Solved by:

- changing package.json to https://github.com/johnpapa/angular2-tour-of-heroes/blob/master/package.json
- installing tsd globally "npm install tsd -g"
- adding "C:\Windows\System32" to PATH variable in cmd which was missing and was likely culprit for the crash. Other two changes   are likely unnecessary 
