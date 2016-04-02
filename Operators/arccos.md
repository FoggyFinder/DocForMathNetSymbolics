#Operators.arccos

	val arccos : x : Expression ->  Expression


#####CompiledName: arccos


####Описание

Возвращает арккосинус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.arccos exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    acos(4*x)




