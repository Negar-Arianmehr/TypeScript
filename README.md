# TypeScript
Adding info during learning TypeScript with Linkedin Course https://www.linkedin.com/learning/learning-typescript-2/understanding-type-inference-and-gradual-typing

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

With typeScript we can assign the variable to type of them. Once the type has been spesified, the display name variable will always be a that kind type. There are seven primitive types built into JavaScript(String, Boolean, Number, Biglnt, Null, Undefined, Symbol...Object). We also can define the structure of object in opening and closing cury bracket.

TypeScript contain two features that allow you to dramatically reduce the code that you have to write in order to take advantage of strong typing and they are called type inference and gradual typing.
Type inference simply means that TypeScript is really smart, and is able to figure out the type of many variables wothout you having to provide any information at all.
TypeScript is a superset of JS, and JS is a dynamice language which means that in JS it is entirely possible to do things like assigning a variable to a number value and reassigning it to the string value. This is where gradual typing comes into play. in other words, type inference allows TypeScript to find errors in your code at compile time by automatically discovering type info like this.
We have any for type of variable that is essentially entirely opting out of type safety and TypeScript's ability to help you. But it has to be last choice(It is not a good thing).
The more information you can give TypeScript, the better it can help you.

For define the Interface, we have to use interface keyword, after that a name that we want.
