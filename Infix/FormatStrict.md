#Infix.formatStrict

	val formatStrict : expression : Expression ->  String


#####CompiledName: FormatStrict


####Описание:
	
Выводит точное представление дерева выражения.

----------

####Пример
    
    let str = "4*x*x + 2/sin(3*y) + 5*cos(x)"
    let expr = str |> Infix.parseOrUndefined
    expr |> Infix.formatStrict |> printfn "%s"

#####Вывод

    4*x^2 + 2*sin(3*y)^(-1) + 5*cos(x)

----------

####Дополнительная информация

Схожесть с функцией [Infix.format](Format.html) может ввести в заблуждение, что они делают одно и то-же. На самом деле это не так. Разницу легко понять, если вывести дерево выражений не используя форматированный вывод:

    let some = "tan(x)/sin(y)"
    let expr = some |> Infix.parseOrUndefined 
    
    expr |> printfn "%A"
    
    expr |> Infix.format |> printfn "Infix.format: %s"
    expr |> Infix.formatStrict |> printfn "Infix.formatStrict: %s"

#####Вывод

    Product
      [Power (Function (Sin,Identifier (Symbol "y")),Number -1N);
       Function (Tan,Identifier (Symbol "x"))]
    Infix.format: tan(x)/sin(y)
    Infix.formatStrict: sin(y)^(-1)*tan(x)


Легко заметить, что Infix.printStrict просто выводит дерево выражения без дополнительных изменений.

