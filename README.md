# ALang-Spec
*ALang doesn't actually do anything, this is the language's idea*

-----------------------
### Vars
*integers, floats and strings are all one has in ALang*
`atom` is the universal mutable variable declaration keyword 
`atom /*identifier*/ = /*value*/;`
`atom x = 10i;` -> the `i` refers to integer
`atom y = 10.0f` -> the `f` refers to float
`atom z = "";` -> this is a string

`const atom` is the universal immutable variable declaration keyword

------

### functions 

``` Alang
func i():
// do something
;
```
Alang uses Indentation but terminates the code block with a lonely semicolon

#### Async Function
``` Alang
async func o(): 
await /*value*/:
// do something
;
```


``` Alang
i() // function call

// capture

i().return = Z;
```

------------

### for loops

#### for loops if the var is not declared

``` Alang
for:
atom X = 0i, X <= 10:
// do something
;

```

#### for loops if the var is declared

``` Alang
for: 
X, X >= 10.0f: 
// logic here
;
```

-----------

### if statements

``` Alang
if: X >= 9.0f: 
 //logic
; else if: X == 10.0f: 
 // logic
; else (NULL): 
 // logic
;
```

----------

### Lists

``` ALang
// anon list

list< 
1. X, 
2. Y, 
3. Z
>;

// identified list

list i<
1. X, 
2. y, 
3. Z
>;

// adding to the list

i<add: "Orange" | column: 3>

// retriving from the list
i<get: item.Banana | column: 2> = Z

// retriving if your don't know what it is
i<column: 2> = Z;

// subtracting from the list

i<remove: item.Orenge | column: 3>

// removing when you don't know what it is

i<remove: column: 3>
```
------

### Map

``` Alang
// maps
map User: 
"name" = "UserName",
"ID" = "10"
;
```

maps have the same access and modify patterns as lists


`User<get: "name", item.UserName> = Z` for instance 
----------




