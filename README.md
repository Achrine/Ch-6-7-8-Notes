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


