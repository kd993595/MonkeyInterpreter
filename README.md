# MonkeyInterpreter

Language Interpreter for monkey language written in golang
Follows the book "Writing an Interpreter in Golang" [Book](https://interpreterbook.com/)

Monkey is a small, interpreted or compiled toy programming language with high-level simplicity and easy to write C-like syntax.
The language features:
* Turing-completeness
* expressions like + - * / -(prefix) !(prefix) == != > <
* local and global variables
* functions/closures as first-class objects
* everything is an expression
* arrays [1, 2, 3]
* strings "Hello"
* full unit test coverage
* written in 100% pure Go without external dependencies


Example: Fibbonaci in Monkey
```
let fibonacci = fn(x) {
    if(x == 0) {
        0
    } else {
        if(x == 1) {
			1
		} else {
			fibonacci(x - 1) + fibonacci(x - 2)
		}
    }
}

puts(fibonacci(10))
```
