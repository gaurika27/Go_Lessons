# Variable Types
  - int- stores integers (whole numbers), such as 123 or -123
      - (Default value=0)
  - float32- stores floating point numbers, with decimals, such as 19.99 or -19.99
      - (Default value=0.00)
  - string - stores text, such as "Hello World". String values are surrounded by double quotes
      - (Default value=" ")
  - bool- stores values with two states: true or false
      - (Default value=false)
# Declaring (Creating) Variables
  - ## With the var keyword:
      - var variablename type = value
        - (Note: You always have to specify either type or value (or both).)
  - ## With the := sign:
      - variablename := value
        - (Note: In this case, the type of the variable is inferred from the value (means that the compiler decides the type of the variable, based on the value).)
        - (Note: It is not possible to declare a variable using :=, without assigning a value to it.)

# Difference between var and :=
  |var	    |:=           |
  |:--------|:------------|
|Can be used inside and outside of functions |Can only be used inside functions
|Variable declaration and value assignment can be done separately	|Variable declaration and value assignment cannot be done separately (must be done in the same line)|

# Go Multiple Variable Declaration
  - 1
     ```go
        package main

        import "fmt"

        func main() {
            var a, b, c, d int = 1, 3, 5, 7

            fmt.Println(a)
            fmt.Println(b)
            fmt.Println(c)
            fmt.Println(d)
     }
    ```
  - 2
    ```go
        package main

        import "fmt"

        func main() {
          var a, b = 6, "Hello"
          c, d := 7, "World!"

            fmt.Println(a)
            fmt.Println(b)
            fmt.Println(c)
            fmt.Println(d)
    }    
    ```
  - 3
    ```go
        package main

        import "fmt"

        func main() {
          var (
            a int
            b int = 1
            c string = "hello"
         )

        fmt.Println(a)
        fmt.Println(b)
        fmt.Println(c)
        fmt.Println(d)
    }    
    ```
# Variable naming rules
  - A variable can have a short name (like x and y) or a more descriptive name (age, price, carname, etc.).
  - Go variable naming rules:
    - A variable name must start with a letter or an underscore character (_)
    - A variable name cannot start with a digit
    - A variable name can only contain alpha-numeric characters and underscores (a-z, A-Z, 0-9, and _ )
    - Variable names are case-sensitive (age, Age and AGE are three different variables)
    - There is no limit on the length of the variable name
    - A variable name cannot contain spaces
    - The variable name cannot be any Go keywords

