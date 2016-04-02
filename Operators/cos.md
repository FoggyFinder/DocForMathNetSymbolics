#Operators.cos

	val cos : x : Expression ->  Expression


#####CompiledName: cos


####Описание

Возвращает косинус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.cos exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    cos(4*x)

