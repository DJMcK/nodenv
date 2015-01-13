# NODENV

![](https://dl.dropboxusercontent.com/s/py4mxf4xeztepsj/demo-optimized.gif)

```
npm install -g nodenv
```

```
echo "source $(which nodenv)" >> ~/.bashrc
```

```
nenv -h
```

## Basic Overview

`nenv -a` will look from your current working directory and up the directory tree for a `node_modules/.bin` folder. If found, this with be added to your `PATH` environment variable - in the current context only, not permanent.

The entry will be added at the start of your PATH and therefore `local > global`. Example being `npm install -g module-with-bin` and the same module installed locally, local will win over global while nenv is active.
