#Polynomial.isSquareFree

	val isSquareFree : symbol : Expression -> x : Expression ->  Boolean


#####CompiledName: IsSquareFree


####Описание

Проверяет, является ли полином свободным от квадратов.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "x^5 - x^3 - x^2 + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> Polynomial.isSquareFree x
    |> printfn "%b"
    

####Вывод
    
    1 - x^2 - x^3 + x^5
    false









