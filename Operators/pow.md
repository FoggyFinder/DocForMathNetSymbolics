#Operators.pow

	val pow : x : Expression -> y : Expression ->  Expression


#####CompiledName: pow


####Описание

Возводит ***x*** в степень ***y*** 
    
----------

####Пример
    
    let x = "4*x" |> Infix.parseOrUndefined
    let y = 3Q
    let newExpr = Operators.pow x y
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    64*x^3


