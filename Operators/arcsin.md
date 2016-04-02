#Operators.arcsin

	val arcsin : x : Expression ->  Expression


#####CompiledName: arcsin


####Описание

Возвращает арксинус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.arcsin exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    asin(4*x)




