#Operators.plus

	val plus : x : 'a -> 'a


#####CompiledName: plus


####Описание

Возвращает выражение без изменений
    
----------

####Пример
    
    let x = "5*sin(x)" |> Infix.parseOrUndefined
    let newExpr = Operators.plus x
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    5*sin(x)


