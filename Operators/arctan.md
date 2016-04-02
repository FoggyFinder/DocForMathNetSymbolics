#Operators.arctan

	val arctan : x : Expression ->  Expression


#####CompiledName: arctan


####Описание

Возвращает арккосинус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.arctan exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    atan(4*x)





