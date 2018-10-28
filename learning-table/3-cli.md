# The Command Line Interface

**create-creenv** provides multiple options so that you can set up a project that best fits your needs.

> To install the CLI, please refer to the first section of the learning table [setting up your first project](https://github.com/bcrespy/creenv/blob/master/learning-table/1-setting-up-first-project.md)

> If you are looking for the list of options available with the CLI, please check [create-creenv full documentation](https://github.com/bcrespy/create-creenv#readme)

## 1. Select the project that fits your needs at best 

First step is of course to think about the structure that will fit your project. The *--mode* option lets you select between different projects, listed below :

| Mode name | Description                                                  |
| --------- | ------------------------------------------------------------ |
| default   | This is the default project, installed if a --mode is not provided to the CLI. A simple project, with brief explanations to understand how it works. The core structure is there. |
| demo      | A full showcase of all the creenv modules. The result is simple, yet a lot of modules are included within the code so that you can see how they work. It is recommended to install this project at least once to understand how creenv can be pushed. |
| light     | The lightest possible project, only a file with required method to implement is provided. |

## 2. Install a specific project

If you run `create-creenv`, this will install the default boilerplate. It is the same as running 

```bash
create-creenv --mode default
```

The *--mode* option let's you select the project you want to use. Pretty straightforward

## 3. All the available options 

The options are available in the full documentation of *create-creenv*, available in the [readme of its repo](https://github.com/bcrespy/create-creenv#readme).

## 4. How does it work

When you run the command, a series of task will be executed:

1. You run the command, and depending on its parameters a repo corresponding to your needs will be selected from the list.
2. The repo get cloned into the directory you specified 
3. The packages required for the repo are installed within the project. The script runs `npm install` into the installation directory 
4. The remote to the repo and *.git* folder are removed. Because your project won't be linked to the original repo of the project, git link is removed so that you can start a fresh new project
5. The CLI asks you informations about your project to update the *package.json* accordingly.