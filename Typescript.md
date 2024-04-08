`TYPESCRIPT`

- It is an superset of a JavaScript.

- TypeScript is a typed Javascript.TypeScript adds types to JavaScript to help you speed up the development by catching errors before you even run the JavaScript code.

- It is open sourced.
- bult on top of Js.
- works on nay browser, OS and any environment which runs js.

- Every javascript program is typescript program. if you have javascript code typed it wont have any syntax errors.

- TypeScript is just like a wrapper around javascript.

`WORKING`

- First we need to write code in typescript which then get compiled into javascript code by using TS compiler.

      TYPESCRIPT       ---->        TYPESCRIPT        ------->          PLAIN
                                    COMPILER                          JAVASCRIPT

- It helps to avoid bugs and potential errors by providing typesafty.

- `eg`

      - If you have an `add(a,b)` function in your javascript which takes to parameters and the values of thes paramenters is accepted from the HTML inputs.

      - suppose some one enthers values `10` and `20` these values are treated as a string and it it will result in unexpected output  `1020`.

      - to get rid of that we can give the prefered types in typescript function as `add(a:number,b:number)` now this TS function won't accepts any other input than the numbers and  give the required output.

- `BASIC TYPES`

  - `TYPE ANNOTATION`

  - `VARIABLES`

    - In typescript type annotation is nothing but the specifying the type of the identfiers such as variables, functions, Objects and function parameters.

    - Typescript uses the syntax `<variable_name> : <type>` to ues type annotation.

    - `eg`

                ```ts
                let anyNumber: number;

    - here anynumber is a variable which is annoted as s type number now only the integer/number type of values could be assigned to the anynumber variable if we/anyone tres to assign the value of any othe type the typeScript compiler throws an error.

    - we can also attonate other datatype to variables as below

               ``` ts
               let anyString :string = "we can only assign string type values to this variable";

               let isBoolean: boolean = true; //either true or false could be assign .

    - `ARRAYS`

      - In typeScript when we have to annotate an arras we have to use syntax `<array_name> : <Type>[]`;

      - `eg`

                  ```ts
                  let numberArray : number[] = [2,45,64,2,1]; //ONly numbers/Integers could be stored.

                  let stringArray: string[] = ["It","is","string","array","!"]; // Only strings could be stored.

                  let boolArray: boolean[] = [true,false,true]; //only bollean values could be stored.

    - `OBJECTS`

          - To attonate objects in Typescript use the syntax:

                        ```ts
                        let <object name>: {
                        <property_name> : <type>;
                        <property_name> : <type>
                        };

                        <Object name> = {
                        <property_name> : <typed data>,
                        <property_name> : <type data>
                        }

      - `eg`

                        ```ts
                        let person: {
                           name: string;
                           age: number
                        };

                        person = {
                           name: 'John',
                           age: 25
                        };

    - `FUNCTION ARGUMENTS AND RETURN TYPES`

      - `ARGUMENTS`

            - In typescript we give type to the function  parameters to avoid any bugs i future.
            - Function accepts only the values of type is assigned to it.

            - whether there is one argument or multiple never wright them without -> ().
            - arguments must be encapsulated all the time.


            - We use the syntax below:
                        ```ts
                        let <function_name> : (arument_name:type) => {body};

                  `eg`

                   -     ```ts
                        let sayHello = (hello :string)=>{
                        console.log(hello);
                        }

                        sayHello("Hello typescript")

      - RETURN TYPE

            - As we are accepting some paramters in the function on we use the function for a specific purpose in this case our functions might return some values or not but what if we haven't delcared the return type of any function and in future any other develper tries to assign the returned value of a function which returns nothing,
            - by default the return type of a function is `any` wheter function returns or not we have to explecitly mentioned the return type of the function.-
            - whether it is `void` or anything else.

            - For giving return type to function use  syntax below:
                        ```ts
                        let <function_name> : (arument_name:type):<return_type> => {body};

                  `eg`

                        ```ts
                        let addThem = (a :number,b:number):number=>{
                        return a+b;
                        }

                        const sum = addThem(32,325);
                        //Now if we do
                        typeof sum // its number
