#Operators.csc

	val csc : x : Expression ->  Expression


#####CompiledName: csc


####Описание

Возвращает косеканс заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.csc exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    1/sin(4*x)


