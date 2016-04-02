#Operators.sqrt

	val sqrt : x : Expression ->  Expression


#####CompiledName: sqrt


####Описание

Возвращает квадратный корень заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.sqrt exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    (4*x)^(1/2)


