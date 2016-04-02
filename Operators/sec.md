#Operators.sec

	val sec : x : Expression ->  Expression


#####CompiledName: sec


####Описание

Возвращает секанс заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.sec exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    1/cos(4*x)


