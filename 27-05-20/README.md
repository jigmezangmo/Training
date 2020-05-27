# What Is Webpack?

```
Webpack is a static module bundler (command line tool to creat bundles of assets (code & files)).
Webpack treats all files and assets as modules.
Its main purpose is to bundle JavaScript files for usage in a browser,
yet it is also capable of transforming, bundling, or packaging just about any resource or asset.

```

## Webpack Main Concepts

```
1. Entry
    - Is a module
    - Webpack use to start building its internal dependency graph
    
2. Output
    - Output property instructs webpack where to emit the bundle(s) and what name to use for that file(s)
    - Default value ((./dist/main.js -> for the main bundle) & (./dist -> for other generated files))

3. Loaders
    - By default, webpack only understands JavaScript and JSON files
    - Webpack use loaders to process other types of files and convert them onto valid modules.

4. Plugins
    - Used for any other task that loaders can't do
    - Provides a wide range of solutions about asset management, bundle minimization and optimization..

5. Mode
    - Providing the mode configuration option tells webpack to use its built-in optimizations accordingly.
    - The default value is production.
```

## How Webpack Works

* Webpack bundles all project's modules into a small number of bundles - usually, just one - to be 
loaded by the browser.

* Webpack can be used as a simple task runner. We can create webpack tasks by including the name of our task followed by its instructions in the # Scripts # section of the # package.json # file.
```
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "dev": "webpack --mode development",
  "build": "webpack --mode production"
},
```
* --mode flag to define # dev # and # build # tasks
* (npm run dev) -> run webpack in development mode respectively
* (npm run build) -> run webpack in production mode respectively

