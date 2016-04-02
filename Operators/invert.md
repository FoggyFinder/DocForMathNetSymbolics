#Operators.invert

	val invert : x : Expression ->  Expression


#####CompiledName: invert


####Описание

Возвращает выражение обратное заданному
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.invert exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    (1/4)/x



