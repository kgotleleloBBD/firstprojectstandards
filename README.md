# First Project Standards
The standard for the project

## Reference
https://eslint.org/docs/latest/rules

## Stylistic Standards  
* Camelcase naming convention.  
* No spacing before and spacing after commas.  
* Consistent use of either single quotes in JSX attributes.  
* No spacing before keys and values, spacing after  keys and values in object literal properties.  
* Consistent spacing before and after keywords.  
* Use Unix linebreak style.  
* Require empty lines before comments.  
* Maximum amount of nests must not exceed 4.  
* Maximum line length of 240.  
* Maximum depth that callbacks can be nested must not exceed 4.  
* Constructor names to begin with a capital letter.  
* Empty line after var, let, or const.  
* No Array constructors.  
* No mixed whitespaces and tabs.  
* No multiple empty lines.  
* No trailing spaces.  
* No spaced functions.  
* Semicolons instead of ASI.  
* spacing after semicolons.  
* Enforce a whitespace after the comment literal.  
* Require spacing around infix and unary operators.  
* No spacing inside parentheses. 


## Best Practices  
* Curly braces on the next line.  
* Nocomplexity from 15 and beyond not allowed.  
* No new operators allowed.  
* No operators with functions allowed.  
* Don't allow void operators.  
* Don't allow with operators.  

## ECMAScript 6 (ES6)
* Enforces parentheses around arrow function parameters regardless of arity.  
* Normalize style of spacing before/after an arrow function’s arrow.  
* Flag invalid/missing super() calls.  
* Enforce consistent spacing around * operators in generator functions.  
* Flag modifying variables of class declarations.  
* Disallow reassigning const variables.  
* Disallow duplicate class members.  
* Disallow new operators with the Symbol object.  
* In the constructor of derived classes, if this/super are used before super() calls, it raises a reference error.  
* Disallow unnecessary constructors.  
* This rule is aimed at discouraging the use of var and encouraging the use of const or let instead.  
* If a variable is never reassigned, using the const declaration is better.  
* Require template literals instead of string concatenation.  
* This rule generates warnings for generator functions that do not have the yield keyword.  
* Require or disallow spacing around embedded expressions of template strings.  

## Possible errors  
* Require or disallow trailing commas  
* Disallow assignment operators in conditional expressions  
* Disallow unreachable code after return, throw, continue, and break statements
* Disallow empty block statements  
* Disallow variable or function declarations in nested blocks

## variables
Disallow catch clause parameters from shadowing variables in the outer scope  
If you do not need to support IE 8 and earlier, you should turn this rule off - no-shadow encoumpasses it.  

The purpose of the delete operator is to remove a property from an object. Using the delete operator on a variable might lead to unexpected behavior.  
This rule disallows the use of the delete operator on variables.  

Disallow labels that share a name with a variable  
This rule aims to create clearer code by disallowing the bad practice of creating a label that shares a name with a variable that is in scope.  

Disallow variable declarations from shadowing variables declared in the outer scope  

Disallow the use of variables before they are defined  
Variables that are declared and not used anywhere in the code are most likely an error due to incomplete refactoring. Such variables take up space in the code and can lead to confusion by readers  

This rule can help you locate potential ReferenceErrors resulting from misspellings of variable and parameter names, or accidental implicit globals (for example, from forgetting the var keyword in a for loop initializer).  

ES5 §15.1.1 Value Properties of the Global Object (NaN, Infinity, undefined) as well as strict mode restricted identifiers eval and arguments are considered to be restricted names in JavaScript.   
Defining them to mean something else can have unintended consequences and confuse others reading the code. For example, there’s nothing preventing you from writing:  
Then any code used within the same scope would not get the global undefined, but rather the local version with a very different meaning.  

## strict
A strict mode directive is a "use strict" literal at the beginning of a script or function body. It enables strict mode semantics.  
When a directive occurs in global scope, strict mode applies to the entire script.  
When a directive occurs at the beginning of a function body, strict mode applies only to that function, including all contained functions.  

JavaScript's strict mode is a way to opt in to a restricted variant of JavaScript, thereby implicitly opting-out of "sloppy mode". Strict mode isn't just a subset: it intentionally has different semantics from normal code. Browsers not supporting strict mode will run strict mode code with different behavior from browsers that do, so don't rely on strict mode without feature-testing for support for the relevant aspects of strict mode. Strict mode code and non-strict mode code can coexist, so scripts can opt into strict mode incrementally.

Strict mode makes several changes to normal JavaScript semantics:

Eliminates some JavaScript silent errors by changing them to throw errors.  
Fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode.  
Prohibits some syntax likely to be defined in future versions of ECMAScript.  
