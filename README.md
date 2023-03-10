# First Project Standards
The standard for the project

## Reference
https://eslint.org/docs/latest/rules

## Stylistic Standards  
* Camelcase naming convention.  
* No spacing before, spacing after commas.  
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
* Spacing after semicolons.  
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
* Disallow trailing commas  
* Disallow assignment operators in conditional expressions  
* Disallow unreachable code after return, throw, continue, and break statements
* Disallow empty block statements  
* Disallow variable or function declarations in nested blocks  
* Disallow reassigning exceptions in catch clauses  
* Disallow constant expressions in conditions  
* Disallow control characters in regular expressions  

## Variables
* no-shadow: Disallow variable declarations from shadowing variables declared in the outer scope.
* no-catch-shadow: Disallow catch clause parameters from shadowing variables in the outer scope  
** If you do not need to support IE 8 and earlier, you should turn this rule off - no-shadow encoumpasses it.  
* no-shadow-restricted-names: Disallow variable declarations from shadowing restricted identifiers. 
* no-undef: Warn and locate potential ReferenceErrors to an undeclared variable. 
* no-unused-vars: Eliminate unused variables, functions and function parameters. 
* no-use-before-define: Disallow the use of variables before they are defined.
* no-delete-var: This rule disallows or warns the use of the delete operator on variables.  
* no-label-var: Disallow labels that share a name with a variable to make clearer code. 
 
