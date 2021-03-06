# dat

Share datasets on The Internet. This is the Dat 1.0 Pre-release candidate.

Key features:

  * **easily share large files** without having to copy them to a central server first
  * **sync incrementally** between machines
  
**Please note** that previous versions of Dat (alpha, beta) are incompatible with the 1.0 pre-release.

## Install

**The current work in progress is not on npm yet**

For now, if you are adventurous and want to try the 1.0 Pre-release candidate, clone this repository and in a terminal inside of the folder you cloned run this command:

```
npm link
```

This should add a `dat` command line command to your PATH. Now you can run `$ dat` to try it out.

## Build Status

Windows        | Mac/Linux
-------------- | ------------
[![Build status](https://ci.appveyor.com/api/projects/status/s236036xnglo4v5l)](https://ci.appveyor.com/project/maxogden/dat) | [![Travis](http://img.shields.io/travis/maxogden/dat.svg?style=flat)](https://travis-ci.org/maxogden/dat)

## Example

Go into a directory and type

```
$ cd mydata/
$ dat share
bd3423sdf2342ksdjf238422k3
```

You are now publishing that data from your computer and it will be publicly accessible as long as your terminal is open. Your friend can get that data like this:

```
$ dat bd3423sdf2342ksdjf238422k3
```

It will start downloading the data into the current location. It will also seed that data as long as the terminal is open.

## Overview

This is the Dat 1.0 Pre-release candidate. We want to make Dat into a data versioning, forking, and syncing tool. The first feature set we are working on is easy file synchronization. Dat embraces the Unix philosophy: a modular design with composable parts. All of the pieces can be replaced with alternative implementations as long as they implement the abstract API.

We would really appreciate your feedback.

**Have questions or suggestions?** Join `#dat` on [freenode](https://webchat.freenode.net) or [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/datproject/discussions?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge). Chat logs are [available here](https://botbot.me/freenode/dat/)
