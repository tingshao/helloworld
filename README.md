## Librealsense2 node.js wrapper
`node-librealsense2` is a node.js wrapper of the library working with Intel® RealSense™ depth cameras (D400 series and the SR300).

## Install Prerequisites
[node.js](https://nodejs.org/) and [node-gyp](https://github.com/nodejs/node-gyp) need to be installed.

### 1. Install node.js
Obtain [a `Node.js` copy](https://nodejs.org/en/download/)

### 2. Prerequisites for install node-gyp

#### For Windows 10
   
Setup prerequisites for `node-gyp` by running the following command in shell, make sure you're running it via "`Run as Administrator`" menu:

```
npm install --global --production windows-build-tools
```

You will probably need to setup [proxy of npm](https://docs.npmjs.com/misc/config#proxy) or [https proxy of npm](https://docs.npmjs.com/misc/config#https-proxy)

You might need to manually fix Python (currently 2.7.xx) installation done by the command above, Run Python installer, choose "`Change Python 2.7.xx`" and then make sure "`Add python.exe to Path`" is checked. Click "`Finish`" to do the fix.

Alternatively, you can read the [offical installation guide](https://github.com/nodejs/node-gyp/blob/master/README.md)

### 3. Install `node-gyp`

```
npm install -g node-gyp
```

Note: specify "`-proxy=http://example.com:<port>`" if node-gyp failed to download file with name pattern "`node-v*-headers.tar.gz`"

## Install from npmjs.com
```
$ npm i --save node-librealsense2
```

## Install from source
```
git clone ...
cd wrappers/nodejs
npm install
```

## Examples
```
$ cd wrappers/nodejs/examples
$ npm install

# Plugin the camera into you machine and run below commands to see if it works
$node nodejs-capture.js
```

## Document
HTML format documents are under wrappers/nodejs/doc which were generated by jsdoc.
