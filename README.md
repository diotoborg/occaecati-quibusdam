[![npm Package](https://img.shields.io/npm/v/@diotoborg/occaecati-quibusdam.svg)](https://www.npmjs.org/package/@diotoborg/occaecati-quibusdam)
[![License](https://img.shields.io/npm/l/@diotoborg/occaecati-quibusdam.svg)](https://github.com/diotoborg/occaecati-quibusdam/blob/master/LICENSE)
[![CodeQL](https://github.com/diotoborg/occaecati-quibusdam/actions/workflows/actions.yml/badge.svg)](https://github.com/diotoborg/occaecati-quibusdam/actions/workflows/actions.yml)
[![Node.js CI](https://github.com/diotoborg/occaecati-quibusdam/actions/workflows/node.js.yml/badge.svg)](https://github.com/diotoborg/occaecati-quibusdam/actions/workflows/node.js.yml)

[![NPM](https://nodei.co/npm/@diotoborg/occaecati-quibusdam.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/@diotoborg/occaecati-quibusdam/)


@diotoborg/occaecati-quibusdam is an extension of the node logging package log4js. Tags can be created and used independently or in combination with other tags; the output can be directed to both a local file, console, datadog, combinations of both on the fly or none. Each tag itteration is incremented.

---------

Included object processing:

* queueObj - Support for dynamic objects with all the tagline appenders 
* queueJson - depreciated. All appenders have been moved into queueObj. See the example tests.

Included tag appenders:

* route - to display path or service name
* line - displays file name and line number
* action - displays action name
* stopwatch - displays time elapsed for a particular tag.
* counter - displays counts applied to a tag.
* error - displays an error message from the try/catch block along with the class/function if available from the stack, or simply display an error message.
* class_function - display the class and function name.
* display - ability to turn tags on or off
* counter - count how many itterations a tag has been inputted to. Helpfull in turning tags on/off.
* datadog - for metrics including increment, incrementBy, gauge, histogram, and set.
* email - Appenders and cron settings allows flexible email delivery options

Installation
---------
```
npm install @diotoborg/occaecati-quibusdam
```

Mocha Test
---------
```
npm test
```

General Setup Tests. 
---------
All tests starting with the letter test_q... are examples of queueObj. The letters beginning with test_qj... indicate queueObj Json samples.
```
npm run test_basic
npm run test_qAll    
npm run test_qTopOne
npm run test_qBottomOne
npm run test_qFuncAll
npm run test_qStatusMatching
npm run test_qNonStatusMatching
npm run test_qVersionMatching
npm run test_qVersionNonMatching
npm run test_qNameMatching
npm run test_qNameNonMatching
npm run test_qjAll
npm run test_qjTopOne
npm run test_qjBottomOne
npm run test_qjFuncAll
npm run test_qjStatusMatching
npm run test_qjStatusNonMatching
npm run test_qjNameMatching
npm run test_qjNameNonMatching
npm run test_qjVersionMatching
npm run test_qjVersionNonMatching

```
