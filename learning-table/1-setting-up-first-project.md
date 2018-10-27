# Setting up your first project

> Welcome to the first part of the learning table. In this section you will learn how to install a creenv project on your machine. Let's dive in :) 
>
> **If you are already familiar with the Javascript ecosystem, [you can jump to part 6]()**

## 1. Find a terminal

If you're on an UNIX based system, good for you a great terminal is already built-in. If you're on windows, you can either use the built-in console, or use an emulator such as [Cmder](http://cmder.net/). I personally recommend the usage of an emulator.

## 2. Install node.js

[Node.js](https://nodejs.org/en/) is a JavaScript runtime built on the top of Chrome's V8 engine. It means it can execute javascript code.

Nodejs comes with a package manager, **npm**. Npm can handle the dependencies of your project, and if you're not familiar with that you first learn how npm works before trying to go further on. However, it's not *required* for you to know all the existing tricks of npm, but still the basics could be great.

[What is npm?](https://docs.npmjs.com/getting-started/what-is-npm)

## 3. Install create-creenv globally 

*create-creenv* is the CLI (Command Line Interface) which installs and sets up a creenv project for you. In order for you to be able to use it anywhere on your computer, you will need to *install it globally* using npm. Open your terminal, and run the following command anywhere:

```bash
npm install -g create-creenv
```

Now *create-creenv* is installed on your computer and you will be able to run it. To try it, you can run

```bash
create-creenv -v
```

Expected output:

```bash
insert here the rsult of the command 
```

*If you don't see such a result on windows, it might be required for you to restart your terminal before being able to run create-creenv*

## 4. Create a creenv project, your project

First, navigate to the directory within which you want your project directory to be:

```bash
cd /path/to/your/folder
```

Then 

```bash
create-creenv your-project-name
```

Where *your project name* is the name of your project and will be the folder in which your project gets installed. The CLI should ask you a few questions about your project before starting the installation. **Then, it begins**. 

You can test if everything is working by going into the project root and starting the development server. It is not required for you to know what the development server is now:

```bash
cd your-project-name
npm run start
```

If your browser opens to a page looking like this:

<insert boilerplate image here>

Your project is set up for using creenv :) !

## 5. Enjoy creenv

Now your project is installed and ready to be used. You should have a */your-project-name* folder at the root of the directory in which you ran `create-creenv your-project-name`. This folder contains the files of your project.

___

# Summup of the commands 

install create-creenv 

```bash
npm install -g create-creenv
```

create a creenv project 

```bash 
cd /path/to/my/folder
create-creenv my-project-name
```

run the development server

```bash
npm run start
```













