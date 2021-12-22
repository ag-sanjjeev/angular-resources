## Angular installation related

npm install -g npm@latest

### angular installation cmd:

npm install -g @angular/cli

### Link ng command to npm:

npm link @angular/cli

### creating new project:

ng new 'project-name'

ng new <project-name> (during project creation choose routing module if multi-page application)

### adding angular theming / material:

ng add @angular/material (install material theme binded with angular)

### creating components:

ng generate component 'path\component-name'

### create service:

ng generate service service-name

### create model class:

ng g class classname --type=model

### serving project

ng serve <-o or --open>

or 

ng serve --port=3000 --open --poll=2000

### Generating router to existing project:

ng g module app-routing --flat --module=app

--------------------------------------------------------------

## Installing modules cmd:

npm install bootstrap --save (this will save package.json also)

but use ng-bootstrap

ng add @ng-bootstrap/ng-bootstrap (if this not work use this => npm i --save @ng-bootstrap/ng-bootstrap --legacy-peer-deps)

npm install jquery --save

npm install popper.js --save

-- after installation & add angular.json --
<pre><code>
      "styles": [

        "node_modules/bootstrap/dist/css/bootstrap.min.css",

        "src/styles.css"

      ],

      "scripts": [

          "node_modules/jquery/dist/jquery.min.js",

          "node_modules/bootstrap/dist/js/bootstrap.min.js"

      ]
</code></pre>
or 

-- use can add cdn directly in index.html --

---------------------------------------------------------------

## Font awesome installation

ref below link: for font-awesome angular:

https://github.com/FortAwesome/angular-fontawesome

ng add @fontawesome/angular-font-awesome@<version>

	if not works use below		

$ npm install @fortawesome/fontawesome-svg-core
$ npm install @fortawesome/free-solid-svg-icons
# See Compatibility table below to choose a correct version
$ npm install @fortawesome/angular-fontawesome@<version>

and import as per documentation

---------------------------------------------------------------


## Avoid not initialised property error

tsconfig.json

"strictPropertyInitialization": false

--------------------------------------------------------------

## Installing AG-Grid for Angular:

install and ag-grid:

npm install --save ag-grid-community ag-grid-angular
npm install # in certain circumstances npm will perform an "auto prune". This step ensures all expected dependencies are | present

and see documentation for implementation...

--------------------------------------------------------------

## If you found something wrong then try out:


clear cache:

npm cache clean --force
npm cache verify

---------------------------------------------------------------