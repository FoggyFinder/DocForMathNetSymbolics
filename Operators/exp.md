#Operators.exp

	val exp : x : Expression ->  Expression


#####CompiledName: exp


####Описание

Возвращает экспоненту заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.exp exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    exp(4*x)


