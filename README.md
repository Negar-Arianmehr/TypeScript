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
Type of Variables:
With typeScript we can assign the variable to type of them. Once the type has been spesified, the display name variable will always be a that kind type. There are seven primitive types built into JavaScript(String, Boolean, Number, Biglnt, Null, Undefined, Symbol...Object). We also can define the structure of object in opening and closing cury bracket.

TypeScript contain two features that allow you to dramatically reduce the code that you have to write in order to take advantage of strong typing and they are called type inference and gradual typing.
Type inference simply means that TypeScript is really smart, and is able to figure out the type of many variables wothout you having to provide any information at all.

TypeScript is a superset of JS, and JS is a dynamice language which means that in JS it is entirely possible to do things like assigning a variable to a number value and reassigning it to the string value. This is where gradual typing comes into play. in other words, type inference allows TypeScript to find errors in your code at compile time by automatically discovering type info like this.
We have any for type of variable that is essentially entirely opting out of type safety and TypeScript's ability to help you. But it has to be last choice(It is not a good thing).
The more information you can give TypeScript, the better it can help you.

Interfaces:
For define the Interface, we have to use interface keyword, after that a name that we want. But intersting part of interface is that interface definitions have no impact on the code that's rendered. These interfaces to remember TypeScript for later and then completely removes them from the code. Interfaces only exist to give TypeScript more information about the code that you're writing and can help you find more mistakes.
We can also use the syntax to define methods as well. There is actually two ways to do that.
In interface we define a method named everything that accept a parameter with specific type. We can also make property optional...For example I want to be able to omit that property entirely like originalNumber?: ...it means that we always have not originalnumber.
Another thing that we can difine on an interface is a readonly property. If you want to change this value, you will get error if it is not the type of readonly that you defined.
enum:
This is stongly typed object that the defines a set of named values. enum actually produce code that can be evaluated at runtime. As defult TypeScript define a value of enum valuess to numbers, incrementing up from zero.
Literal types:
With it you can define the list of possible values, separated by the pipe character as inline character.
Union Type ... | :
like number | string...This syntax tells TypeScript that the original cost variable can be either a number or a string at any given time.
If we want to save this combination of types to reuse somewhere else in my application, I can do that with the type keyword like this.  
Classes:
We need to define the properties. We can also use interface. Static keyword is for define the class.
Access Modifiers in TypeScript:
TypeScript privides us with the ability to hide, or incapsulate some or all of our class members, by using something called Access Modifiers. These Modifiers are (keywords):
private: only visible to members within the same class
protected: Visible to members within the same class and derived classes
public(default) : Visible to all consumers
Generics: 


