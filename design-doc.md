# Basics
Alexandria has simple syntax that is easy for new coders to master. The following text will show the structure of Alexandria, showcasing its syntax, commands, and rules.

---

# Commands
## Variables and Display
In Alexandria, all variables need to be defined before declaring its value or using it in a project.

`
ln(text)
`
- ln() is used for string variables.
- You can not directly print text in Alexandria, you need a variable first. Then, use view(var) to display the text.

`
teger(int)
`
- teger() is used for numerical variables only.
- You can include a teger variable inside a ln variable (or really any variable) by using curly brackets / braces around the variable name (ex. text = the secret # was {secret}.)

`
arith(sum)
`
- arith() is used for arithmetic and other mathematic operations inside a variable.
- There is no need for curly brackets inside an arith variable. (ex.

`
arith(sum)
 sum = x + y
`
)

`
view(var)
`
- In Alexandria, you can not direectly print text, integers, etc. You must give a variable a value, and then view the variable.
- Similar to "print" in other languages.

## Conditionals
`
if condition()
`
- Executes if the condition is met.

`
else()
`
- Executes if the condition is **not** met.

`
boolean(name)
`
- Assigns a true or false statement.

## Loops

`
until condition()
`
- Repeats what it inside the parentheses until the condition is met.

`
x(+)
`
- Increases the value of x by 1.

`
x(-)
`
- Decreases the value of x by 1.

## Lists
`
map(name)
`
- Creates a list of items.
- Example:
```
map(fruit)
  fruit = apple, banana, orange
```


`
num.mapname
`
- Finds the nth item in a list.
- Alexandria starts with 0 for lists.
- Example: view(0.fruit)
 - Will display "apple"

## Classes and Functions
`
class(name)
`
- Defines a class
- Any variables used in a class **must** be defined in said class.

`
class(name.Instance)
`
- Makes an object in the class.
- Can be reused later.

`
function(name)(action)
`
- Creates a function.
- Used inside classes to do a callback later.
- Without the action section (if the function is already defined), it will run the function.

`
adapt(x)
`
- Returns a numerical value.
- **Requires** an expression underneath to work.

---

This section is pretty confusing, so here are two **examples of classes, functions, and adapt**.

### Classes / Functions

```
class(work)
 ln(name)
 teger(year)
 ln(job)
 ln(text)

 function(work)(
  text = hello, i am {name} and I worked at {job} for {year} years.
  view(text)
 )

class(work.Bob)
 name = Bob
 year = 5
 job = the local supermarket
 function(work)
```
**Display**: 
`
hello, i am Bob and I worked at the local supermarket for 5 years.
`

### Adapt
```
teger(x)
x = 5

teger(square)

adapt(square) # In this instance, can be replaced with `arith(square)`
 square = x * x


view(square)
```
**Display**:
`
25
`

## Miscellaneous
`
ask(text)
`
- Asks the user "text" and waits for input.

`
x = input
`
- Stores the input in a variable.

`
i = random(x,y)
`
- Chooses a number between x and y. (Variables are supported)
