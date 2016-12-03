# angular2
angular2 sample applications and seeds

### Pre-requisites

\# | Type | Name | Version | Download
---|------|------|---------|------|
1  | JS Server | NodeJS | 4.1+ | https://nodejs.org/en/ |
2  | JS Build | GulpJS | 4.0+ | http://gulpjs.com/ |
3  | JS library | Bower | 1.7+ | https://bower.io/ |
4  | TS module | Typescript | 2.0 | https://www.typescriptlang.org/ |
5  | Atom | editor | 1.12.6 | https://atom.io/ |

#### Hello world Sample:

Writing your first hello world sample of the angular2, clone this git or download.

```
$ git clone https://github.com/uttesh/angular2.git
$ cd a2_hello_world
```
Your a2_hello_world directory look  something like this:
```
#!bash  
/${angular2_HOME}
	|- /a2_hello_world
    |- node_modules/      // installed dependencies
    |- typings/         // type script configuration
    |- app-name.ts        // app component
    |- app.ts             // app module
    |- index.html         // index.html
    |- package.json       // npm libraries
    |- styles.css         // styles
    |- systemjs.config.js // helper to load the modules and dependencies
    |- tsconfig.json      // compiler configuration
    |- typings.json       // ts registry with ec6-shim
```

### Angular’s Dependencies

To run the angular2 four dependencies libraries are there.
<ol>
<li>core-js</li>
<li>zone.js</li>
<li>reflect-metadata</li>
<li>SystemJS</li>
</ol>

We need to add dependencies libraries in the <head> tag of index.html

```
<!-- Libraries -->
<script src="node_modules/core-js/client/shim.min.js"></script>
<script src="node_modules/zone.js/dist/zone.js"></script>
<script src="node_modules/reflect-metadata/Reflect.js"></script>
<script src="node_modules/systemjs/dist/system.src.js"></script>
```

Why shim.min.js ? </br>
Latest chrome and FF browser its not required, but to support some of the features on the older version browser, we need poly fills which will help in the backward capabilities for some extend.

Why zone.js ? </br>
Library used by Angular, primarily for detecting changes to data.

Why Reflect.js ? </br>
This Library is a polyfills which will help in the metadata i.e. annotation of typescript in angular2.

why system.src.js ? </br>
it's a module loader. Helps in create modules and resolve dependencies.

Running first hello world a2 app.

Step1: install npm modules.
```
$a2_hello_world> npm install
```

Step 2: Compile typescript files i.e. .ts file to generate the respective .js files.

run the TypeScript compiler command line  called tsc

```
$a2_hello_world> tsc
```
same can be run by using npm module.

```
$a2_hello_world> npm run tsc
```

Step 3: serve the application.

```
$a2_hello_world> npm run serve
```
