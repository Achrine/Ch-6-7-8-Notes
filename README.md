# Ch-6-7-8-Notes


## Chapter 6: Modular Programming

* Modular Programming 
    * Breaking a program up into smaller, manageable functions or modules. 
* Function: 
    * A collection of statements to perform a task. 
* Motivation for Modular Programming: 
    * Improves maintainability of programs. 
    * Simplifies the process of writing programs. 

### 6.2 Defining and Calling Funcions. 
* Function call: Statement causes a function to execute. 
* Function definition: Statements that make up a function. 
* Definition includes: 
    * return type: Data type of the value that function returns to the part of the progarm that called it. 
    * name: Name of the function. Function names follow the same rules as variables. 
    * parameter list: Variables containing values passed to the function. 
    * body: Statements that perform the function's task. 
        * enclosed in {}
` 
int main () {
        cout << "Hello world\n";
        return 0;
}
`
#### Function Return Type: 
* If a function returns a value, teh type ofthe value must be indicated: 
* int main()
* If a function does not return a value, its return type is void: 
* 

`void printHeading()`
`
`{`
`    cout << "Monthly Sales\n";`
`}`

#### Calling a Function 
* To call a function, use the function name followed by () and ; 
    * printHeading();
* When called, program executes the body of the called function. 
* After the function terminates, execution resumes in the calling function at poitn of call. 
* `main` can call any number of functions 
* Function can call other functions 
* Compiler must know the following about a function before it is called: 
    * name 
    * return type
    * number of parameters 
    * data type of each parameter.
    
### 6.3 Function Prototypes
* Ways to notify the compiler about a function before a call to the function: 
    * Place function definition before calling functions definition. 
    * Use a function prototype (function declaration) - like the function definition without the body.
        *  Header: void printHeading()
        *  Prototype: void printHeading();
#### Prototype Notes 
* Place prototypes near top of program
* Program must include either prototype or full function definition before any call to the function -- compiler error otherwise
* When using prototypes, can place function definitions in any order in source file. 

### 6.4 Sending Data into a Function 
* Can pass values into a function at time of call: 
    * c = pow (a, b);
* Values passed to function are arguments. 
* Variables in a function that hold the values passed as arguments are parameters. 

#### Other Parameter Terminology 
* A parameter can also be called a formal parameter or a formal argument 
* An argument can also be called an actual parameter or an actual argument
* For each function argument, 
    * the prototype must include the data type of each parameter inside its parantheses 
    * The header must include a declaration for each prameter in its ()
        * void evenOrOdd (int); // prototype 
        * void evenOrOdd (int num) // header
        * evenOrOdd(val); //call
#### Function Call notes
* Value of argumen is copied into parameter when teh function is called 
* A parameter's scope is the function which usess it 
* Function can have multiple parameters 
* There must be a data type listed in teh prototype () and an argument declaration in the function header () for each parameter 
* Argemunts will be promoted/demoted as secessary to match parameters. 


#### Passing Muliple Arguments
* When calling a function and passing multiple arguments: 
    * the number of arguments in the call must match teh prototype and definition 
    * The first argument willbe used to initialize the first parameter, the second argument to initialize the second parameter, etc. 

### 6.5 Passing Data by Value

