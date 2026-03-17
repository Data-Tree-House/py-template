![banner](./assets/banner.svg)

# datatreehouse.org template

[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border-purple.json)](https://github.com/copier-org/copier)

## 📦 Installation

Prerequisites:
1. This is a Python library and you definitely need to have Python 3.9 or newer.
2. You will also require Git 2.27 or newer

Then, you can install *copier* by running the command:

```bash
pip install copier
```

If you're having some problems installing, you can read more about the installation steps on the [copier website](https://copier.readthedocs.io/en/stable/)

## ❓ How to use

In a terminal of choice (I'm just using Windows CMD), run the following command (I'll break it down below)

```bash
python -m copier copy gh:/data-tree-house/py-template path/to/destination/folder
```

A breakdown of what we're doing:
- `python -m copier` will run the `copier` library as a *module* (`-m`)
- We're running the `copy` command. The next two arguments are the `src` (source) and `dest` (destination)
- Our source will be a Github Repository (`gh:/`). More specifically, we're copying from the `data-tree-house/py-template` repository.
- Our destination is simply the path to our project. If your terminal is already in your project folder, you can simply pass a dot (`.`) to say "where I am right now" or you can give the path to a folder. The folder does not have to exist! The library will create the folder for you

Here's an example of how I do it. First I change directory to where I keep all my projects:

```cmd
cd C:\Users\johan\OneDrive\Documents\00_local_repos\
```

then I run the command

```cmd
python -m copier copy gh:/data-tree-house/py-template coffee-analysis
```
and it will create a folder called `coffee-analysis` for me!

After you run this command, a series of questions will be asked. You can have a look at all the questions in the [copier.yml](./copier.yml) file.
