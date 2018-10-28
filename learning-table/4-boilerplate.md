# Boilerplate in details 

> This guide will focus on everything there is to know about the boilerplate installed by *create-creenv*. This guide is based on the **default** boilerplate, but the first parts can be extended to all the boilerplates.

**If you already are familiar with npm and webpack, you can skip parts 2 and 3**

## 1. The file structure 

After installing a creenv project, this is what the directory should look like:

```
├── public
|   ├── index.html
├── src
|   ├── main.js
|   ├── renderer.js
|   ├── ... 
├── webpack
|   ├── dev.config.js
|   ├── prod.config.js
.gitignore
LICENSE
package.json
readme.md
```

### a. The /public folder 

All the files you put in the /public folder will be served to the destination folder. Such a behavior is detailed in the 3rd section of this guide.

### b. The /src folder

This is where the sources of your project are. This is where you will have to write your app. The section 4 describes how is structed a creenv application.

### c. The /webpack folder

The webpack folder contains the config files for both development and production modes. You will probably never have to edit those files.

## 2. NPM and @creenv modules

NPM is a dependencies manager. If you're not familiar with the concept of dependencies or npm, it is recommended but not mandatory that you first learn those topics before diving into creenv.

@creenv modules are npm packages. They are listed within the **package.json** at the project's root, this is how npm knows that it needs to get those modules online at the installation. Once the modules are installed, you can **import** them in the javascript files, therefore gaining access to their code and their functionalities. 