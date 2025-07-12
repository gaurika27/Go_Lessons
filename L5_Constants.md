  - The const keyword declares the variable as "constant", which means that it is unchangeable and read-only.

# Constant Types
  There are two types of constants:
  - Typed constants: Typed constants are declared with a defined type
      
      ```go
      package main
      import ("fmt")

      const A int = 1

      func main() {
        fmt.Println(A)
      }
      ```
      
  - Untyped constants: Untyped constants are declared without a type
      ```go
      package main
      import ("fmt")

      const A = 1

      func main() {
        fmt.Println(A)
      }
      ```
      
