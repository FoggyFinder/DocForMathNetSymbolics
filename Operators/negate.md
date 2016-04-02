#Operators.negate

	val negate : x : Expression ->  Expression


#####CompiledName: negate


####Описание

Возвращает отрицание заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.negate exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -4*x

