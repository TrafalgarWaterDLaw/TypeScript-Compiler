# TypeScript Compiler

-------------------------------------

## Table of contents

- [Overview](#overview)
  - [Watch mode](#watch-mode)
  - [Initialising the project](#initialising-the-project)
  - [Compiler options](#compiler-options)
    - [Strict Type Checking](#strict-type-checking)
    - [Additional Checks](#additional-checks)
- [Debug](#debug)
- [Trivia](#trivia)


**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Watch mode

Constanly having to re-compiler the typescript files is a pain, it becomes tedious over time. The solution is to use watch 
mode, which will re-compile the typescript files when they change. To enter watch mode we can use 

``` 
tsc app.ts --watch 

```
OR 

```
tsc app.ts -w   
   
```

### Initialising the project

In order to watch the entire file system we need to initialise the project. This is done by using the following command:

```
tsc --init

```
The command above will create a `tsconfig.json` file in the root directory of the project. This file contains the
configuration for the typescript compiler.

### Compiler options

- Target is used to set the JavaScript version that you would like your code to compile to. Thge default is ES5.
- Module is used to set the module system that you would like to use. The default is CommonJS.
- SourceMap is used to generate source maps. The default is true.
- SourceRoot is used to set the root directory for the source files. The default is the current directory.
- EmitDecoratorMetadata is used to generate metadata for decorators. The default is true.
- DownlevelIteration is used to enable the downlevel iteration. The default is false.
- ModuleResolution is used to set the module resolution strategy. The default is Classic.
- NewLine is used to set the new line character. The default is \n.
- NoEmitOnError is used to stop the compiler from emitting any files if there are errors. The default is false.
- NoImplicitAny is used to stop the compiler from using the `any` type. The default is false.
- NoLib is used to stop the compiler from generating a default library. The default is false.
- NoResolve is used to stop the compiler from resolving modules. The default is false.
- PreserveConstEnums is used to preserve const enums. The default is false.
- RemoveComments is used to remove comments from the output. The default is false.
- SuppressImplicitAnyIndexErrors is used to suppress the implicit any errors for indexing objects. The default is false.
- CheckJs is used to check the javascript files with the TypeScript compiler. The default is false.
- AllowJs is used to allow javascript files to be compiled. The default is false.
- OutDir is used to set the output directory. The default is the current directory.
- RootDir is used to set the root directory in which the compiler should check for the Typescript files. The default is the current directory.
- RemoveComments is used to remove comments from the output. The default is false.
- noEmit is used to stop the compiler from producing files after compliation. The default is false.
- noEmitOnError is used to stop the compiler from emitting files if there are errors. The default is false. Should be set to true 😉.

#### Strict Type Checking

- Strict, if set to true will enable able all strick type checking. The default is false.
- noImplicitAny, it ensures that any variable must be defined before use. The default is false.
- strictNullChecks, it ensures that they is no value that contains null. Solutions include using the using the `!` operator or setting it's value to false.
- strictFunctionTypes, it ensures that functions are typed correctly. The default is false.
- strictBindCallApply, it ensures that functions are bound correctly. The default is false.
- noImplicitThis, it ensures that this is not used before it's defined. The default is false.
- alwaysStrict, it ensures that all code is in strict mode. The default is false.

#### Additional Checks

- noUnusedLocals, it ensures that all local variables are used. The default is false.
- noUnusedParameters, it ensures that all parameters are used. The default is false.
- noImplicitReturns, it ensures that all return statements have an explicit return value. The default is false.
- noFallthroughCasesInSwitch, it ensures that there are no fallthrough cases in switch statements. The default is false.


## Debug

Use the Debugger for Chrome to debug your code alongside source maps.

## Trivia

Never Thought I would have a repo that mainly consists of a README.md file. 🎊 I'm glad I did.