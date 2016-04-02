#Operators.symbol

	val symbol : name : String ->  Expression


#####CompiledName: symbol


####Описание

Задает символ (Symbol) по заданному имени (строки)
    
----------

####Пример
    
    let x = Operators.symbol "x"
    
    x
    |> Infix.format
    |> printfn "%s"

####Вывод

    x


----------

####Дополнительная информация

В связи с тем, что метод принимает на вход строку, может ошибочно
показаться, что он действует аналогично с группой методов parse из модуля [Infix](./function.html#Infix).
Разница будет очевидна, если выводить результат не через специальный метод, а напрямую:


    let expr = Operators.symbol "3*x+5*y"
    expr
    |> printfn "%A"
    
    expr
    |> Infix.format
    |> printfn "%s"

Вывод:
    
    Identifier (Symbol "3*x+5*y")
    3*x+5*y
