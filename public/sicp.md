Sicp lectures

Videos - https://www.youtube.com/watch?v=-J_xL4IGhJA&t=293s

Reference for newer course - https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/

Introduction

- not actually "computer" "science"
- declarative vs imperation - sq rt example
- process -> procedure -> lisp
- programming = formalize 'how to' of the imperative process
- CS = techniques for controlling complexity of large systems
- CS = deals with abstract entities vs real parts (airline, amplifier)

Techniques

- black box abstraction
  - sq rt - imperative process is encapsulated in the box
  - boxes should be able to take in other boxes as inputs
  - box = procedure = imperative knowledge
- conventional interfaces
  - agreed upon ways of plugging things together
- metalinguistic abstraction
  - how you construct new languages

General framework for thinking about languages
 - what are the primitive elements
 - what are the methods of combination
 - what are the methods of abstraction - to make complicated 'primitive' entities

Lisp
  - 3 = primitive
  - combination
    ```
    (+ 3 12.4 5)
    |-----------| -> combination
    operator and operands make up the combination
    ```
    - prefix notation - helps make the syntax tree
  - abstraction
    - `(define A (+ 5 5))`

    - ```
      (define square (lambda (x) (* x x)))
      ```
      lambda = make a procedure with argument x that returns sqaure
    - case analysis
      ```
        (define (abs x)
          (cond ((< x 0) (- x))
                ((= 0 ) 0)
                ((> x 0) x)
          )
        )
      ```
      ```
        (define (abs x)
          (if (< x 0)
              (- x)
              x)
        )
      ```

