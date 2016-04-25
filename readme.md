# rig-angular
[![Dependency Status](https://david-dm.org/vladfilipro/rig-angular.svg)](https://david-dm.org/vladfilipro/rig-angular)

A rig containing angular utilities

## How to use
1. Install rigs package: `npm install rigs`
2. Install rig-angular: `npm install rig-angular`

## Available tasks in rig-angular
- `rig-angular__templatecache`: A task which generates adds source files into angular template cache. The task outputs a javascript file with pre-generated angular code.
  - properties:
    - `src`: String or Array, represents the files to be injected into template cache
    - `dest`: String or Array, represents the output directory
    - `filename`: String representing the output filename
    - `options`: Object, representing the [gulp-angular-templatecache](https://www.npmjs.com/package/gulp-angular-templatecache) configuration

    ```
    {
        taskname: 'rig-angular__templatecache',
        dependency: [],
        src: './src/**/*',
        dest: './tmp',
        filename: 'templates.js',
        options: {
            module: require( path.resolve( './package' ) ).name + '-templates',
            standalone: true,
            moduleSystem: 'Browserify'
        }
    }
    ```

### Generated using [webcase-rig](https://www.npmjs.com/package/webcase-rig) version 1.0.1
