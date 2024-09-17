1. Написать программу, которая определяет, является ли введенное пользователем число четным или нечетным.

2. Реализовать функцию, которая принимает число и возвращает "Positive", "Negative" или "Zero".

3. Написать программу, которая выводит все числа от 1 до 10 с помощью цикла for.

4. Написать функцию, которая принимает строку и возвращает ее длину.

5. Создать структуру Rectangle и реализовать метод для вычисления площади прямоугольника.

6. Написать функцию, которая принимает два целых числа и возвращает их среднее значение.

```
  package main
  
  import "fmt"
  
  //task_1
  func main() {
  
  	var num int
  
  	fmt.Print("\nEnter the value: ")
  
  	fmt.Scan(&num)
  
  	fmt.Print("\n1st task\n")
  	if num%2 == 0 {
  		fmt.Print("even")
  	} else {
  		fmt.Print("odd")
  	}
  	WhatIsNum(num)
  	Foreach()
  }
  
  //task_2
  func WhatIsNum(a int) {
  	fmt.Print("\n\n2nd task\n")
  	if a > 0 {
  		fmt.Print("Positive")
  	} else if a == 0 {
  		fmt.Print("Zero")
  	} else {
  		fmt.Print("Negative")
  	}
  }
  
  //task_3
  func Foreach() {
  
  	var myString string
  
  	fmt.Print("\n\n3rd task\n")
  	for i := 1; i <= 10; i++ {
  		fmt.Print(i, " ")
  	}
  
  	fmt.Print("\n\n4th task\nEnter text: ")
  	fmt.Scan(&myString)
  	StringNum(myString)
  }
  
  //task_4
  func StringNum(a string) {
  	fmt.Print("lenght ", "'", a, "'", " is - ", len(a))
  	ForRect()
  }
  
  //task_5
  type Rectangle struct {
  	a float64
  	b float64
  }
  
  func ForRect() {
  	fmt.Print("\n\n5th task\n", "enter two sides of rectangle:\n")
  
  	var a1 float64
  	var a2 float64
  
  	fmt.Scan(&a1, &a2)
  
  	rectangle := Rectangle{a: a1, b: a2}
  	fmt.Print("rectangle area is - ", rectangle.a*rectangle.b)
  
  	MultNum(int(a1), int(a2))
  }
  
  //task_6
  func MultNum(a int, b int) {
  
  	averageValue := float64((float64(a) + float64(b)) / 2)
  	fmt.Print("\n\n6th task\n", "AverageValue is ", averageValue)
  
  }

```
