---
title: For Loop
localeTitle: Для цикла
---
# Для цикла

Цикл `for` дает вам компактный способ итерации по целому ряду значений. Базовый `for` оператора состоит из трех частей: инициализации переменных, булевского выражения и выражения инкремента.

```java
for (variable initialization; boolean expression; increment expression) 
 { 
    // Statements 
 } 
```

*   `initialization` - инициализирует цикл и выполняется только один раз, в начале.

Вы можете инициализировать более одной переменной того же типа в первой части основных `for` декларации контура; каждая инициализация должна быть разделена запятой.

*   `expression` - оценивается в начале каждой итерации. Если `expression` оценивается как `true` , `Statements` будут выполнены.
*   `increment` - вызывается после каждой итерации через цикл. Здесь вы можете увеличить / уменьшить значение переменных. Убедитесь, что приращение работает над значением выражения, чтобы избежать бесконечного цикла.

Общим способом использования цикла `for` является то, что вам нужно повторять ваш код определенное количество раз. Например, если вы хотите вывести числа 0-10, вы должны инициализировать переменную для вашего счетчика равным 0, а затем проверить, меньше ли это значение 10, и добавить один к счетчику после каждой итерации.

Обратите внимание, что вы проверите, будет ли значение меньше 10, не менее или равно 10, так как вы начинаете свой счетчик с 0.

```java
for (int iter_For = 0; iter_For < 10; iter_For++) 
 { 
    System.out.print(iter_For + " "); 
    // Iterated 10 times, iter_For 0,1,2...9 
 } 
 
 System.out.println("iter_For Value: " + iter_For); 
```

Примечание. Также допустимо объявить переменную в цикле for как один оператор.

```java
for (int iter_For = 0; iter_For < 10; iter_For++) 
 { 
    System.out.print (iter_For + " "); 
    // Iterated 10 times, iter_For 0,1,2...9 
 } 
```

Вывод:
```
0 1 2 3 4 5 6 7 8 9 
 iter_For Value: 10 
```

Другой пример цикла for, который добавляет первые 50 номеров, будет таким. i ++ означает i = i + 1.

```java
int addUntil = 50; 
 int sum 0; 
 
 for (int i = 1; i <= addUntil; i++) 
 { 
    sum+=i 
 } 
 
 System.out.println("The sum of the first 50 numbers is: " + 50); 
```

![:rocket:](https://forum.freecodecamp.org/images/emoji/emoji_one/rocket.png?v=2 ": Ракета:") [Код запуска](https://repl.it/CJYr/0)

### Дополнительно

Вы не можете использовать число (старая конструкция языка C-стиля) или что-либо, что не оценивает логическое значение как условие для оператора if или цикла. Вы не можете, например, сказать if (x), если x не является логической переменной.

Кроме того, важно иметь в виду, что булево выражение должно в какой-то момент оценить значение true. В противном случае ваша программа застрянет в бесконечном цикле.