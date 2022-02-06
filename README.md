# Core-Code


# Week challenges (tuesday)

Q1.  Java language is compiled or interpreted?

R: It can be considered to be an interpreted and compiled language,
because it is first compiled and then executed in the java virtual machine, which is usually an interpreter.

Q2. Create an algorithm to calculate the equivalent of your local currencty to USD.


Q3. Anwser to the question: Why is pseudocode helpful?

R: Pseudocode is helpful because it helps our mind to come up with a strategy 
on how to create a program or a function in a programming language.

Q4. Create a pseudocode to calculate the aproximated age of a user base on the year they born.

R:  Pseudocode CalcularEdad
    Variable: current_year (2022)
    Int year_birth
    Int edad
    Start
    Solicitar (“ingrese el año de nacimiento”)
    Leer (year_birth)
    Mostrar (edad = current_year – yearbirth)
    Fin.

Q5. Answer to the question: Why are flowcharts important to us as developers?

R: son importates ya que se pueden utilizar como una representación visual del flujo de datos,
los diagramas de flujo son útiles para escribir un programa o algoritmo y explicárselo a otros o colaborar con otros.


# Week challenges (wednesday)

Q1. Translate the year you where born to binary, decimal and hexadecimal.

R: year of birth= 1994
Binary = 11111001010
decimal = 1994
hexadecimal = 7CA

Q2. Translate 51966 into hexadecimal and binary.

R: Binary= 1100101011111110
Hexadecimal = CAFE

Q3. 5.1 Create a program to add two numbers given by the user.

	.data
		number1: .asciiz "\nIngrese el primer numero: "
		number2: .asciiz "\nIngrese el segundo numero: "
		suma:  .asciiz "\nLa suma es: "
	.text
		main:
			li $v0, 4
			la $a0, number1
			syscall

		li $v0, 5
		syscall
		move $t0, $v0

		li $v0, 4
		la $a0, number2
		syscall

		li $v0, 5
		syscall
		move $t1, $v0

		Add $t3,$t0,$t1

                li $v0,4 
                la $a0, suma
                syscall

                li $v0,1
                 move $a0,$t3 
                 syscall

                li $v0,10 
                syscall

		li $v0, 1
		move $a0, $t0
		syscall

Q4. 5.2 Create a program that display your name.

.data
    message: .asciiz "\nMi nombre es: Josue Rivera\n"
  .text
    main:
      li $v0, 4
      la $a0, message
      syscall


# Week challenges (Thursday)

Q1. Search for real word applications of Javascript

Q2. Follow the github course.

# Week 2 Javascript
## Week challenges (Monday)

Q1. Follow the github course. Done
Q2. Watch this video. Done
Q3. Read this. Done
Q3. Create an account in Codewars. Done

## Week challenges (Monday)
Q0. Watch this video. Done
Q1. https://www.codewars.com/kata/50654ddff44f800200000004 (Multiply)
	function multiply(a, b){
	  return a*b
	}

Q2. https://www.codewars.com/kata/572b6b2772a38bc1e700007a (ASCII Total)
	
	function uniTotal (string) {
	 let suma=0;
	  for(var i=0; i<string.length;i++){
	    suma=suma+string.charCodeAt(i);
	  }
	  return suma;
	}
		
	
	
Q3. https://www.codewars.com/kata/55ad04714f0b468e8200001c  (get character from ASCII Value)

	function getChar(c){
	  let char = String.fromCharCode(c);
	   return char;
	}


Q4. https://www.codewars.com/kata/551f37452ff852b7bd000139  (Binary Addition)
	
	function addBinary(a,b){
	  let add = a+b;
	  let cB= add.toString(2);
	  return cB;
	}
	console.log(addBinary(5,3))
	
Q5. https://www.codewars.com/kata/5ad0d8356165e63c140014d4 (Student's Final Grade)
	




