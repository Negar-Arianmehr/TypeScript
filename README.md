# TypeScript
Adding info during learning TypeScript with Linkedin Course

First steps for coding with TypeScript:
1. We need typeScript Compiler we can find that at typescriptlang.org
2. We will be using the Node.js instructions (You can check that you have the Node.js in terminal with typing: npm -v)
So now we can install typescript via npm: npm install typescript. Now write npx tsc...by writing command tsc

Next thing that we have to do is to add typscript to the application. The only thing that I need to do is add the TypeScript configuration file into the root of Project.
This file must be called tsconfig.json. The content of this file will be a JSON object which contains all of our settings. This configuration object takes a handful of top-level properties, and most important one is compilerOptions, which itself has another object containing a set of properties you can see in codes.
For instant, target is one of properties of compilerOptions that spasify which ECMAScript version the code that it outputs must be compatible with. We use target "es5" that with virtually every browser in use today.
With this target We can show how TypeScript manipulates the code during the transpilation process.
Second option is "outDir" : This option tells the TypeScripte compiler where it should save the transpiled JavaScript it produces.
When we type tsc -w in the terminal, that the w stand for watch.

In this part we have model.ts and in dist we have model.js. When we write some part of code in model.ts and save it we can see the output the TypeScript transpiler in the model.js file. 

