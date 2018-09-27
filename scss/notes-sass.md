# Notes for SCSS

- main.scss file will be the main scss file, all the other files will be partials and will be imported into main.scss file.
- we need a way for our sass to be compiled into css files, because the browser does not understand scss files.

  - so we have to use node sass.
  - in order to install node sass we need to use npm, -> _npm install node-sass_
  - before installing node-sass we need to create _package.json_ file, which serves as a manifest for our project. And to do that we can do **npm init** in the terminal. Fill out the necessary information and follow the instructions.
  - if we install anything with _npm_, it will get put in this file inside the dipendencies object.
  - after that we can install node-sass. What it is going to do is create a _node_modules_ folder anytime you install something with _npm_ it will be installed into node_modules folder.
  - after downloading it we need to make it work. In _package.json_ there is something called **scripts** object. There we need to change test to sass and value to "node-sass -w scss/ -o src/scc --recursive". where **-w** watches for changes in scss folder and **-o** outputs it into _src/css/_ folder.
