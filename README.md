# modern-workflow-demo

[![Join the chat at https://gitter.im/remojansen/modern-workflow-demo](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/remojansen/modern-workflow-demo?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://secure.travis-ci.org/remojansen/modern-workflow-demo.png?branch=master)](https://travis-ci.org/remojansen/modern-workflow-demo) [![Dependencies](https://david-dm.org/remojansen/modern-workflow-demo.png)](https://david-dm.org/remojansen/modern-workflow-demo#info=dependencies)

A TypeScript + Sass + Browserify + Gulp + Karma + BroserSync demo repository

## Workflow

1. **lint**: Lints JSON under ``./data``,  TypeScript under ``./source/ts/`` ``./test``and Sass under ``./source/scss/``.

        gulp lint

2. **build**: Compiles Sass and TypeScript files from ``./source`` to ``./temp``.

        gulp build

3. **bundle**: Bundle files from ``./temp`` to ``./dist`` powered by Browserify.

        gulp bundle

4. **test**: Run Mocha + Chai + Sinon unit test powered by Karma.

        gulp test

5. **serve**: Host app in static server and  refresh browser on changes powered by BrowserSync.

        gulp serve

The default task will run  

    gulp.task('default', ['lint', 'build', 'bundle','test']);  

There are two additional tasks:

1. **install**: Re-installs ``bower_components``, ``node_modules`` and ``typings``.

        gulp install

2. **clean**: Deletes the ``./temp`` and ``./dist`` directories.

        gulp clean


## License

MIT
