#Operators.multiply

	val multiply: x : Expression -> y : Expression ->  Expression


#####CompiledName: multiply


####Описание

    Возвращает произведение двух выражений
    
----------

####Пример

    let x = "-3*x" |> Infix.parseOrUndefined
    let y = "5*y*sin(x)" |> Infix.parseOrUndefined
    
    let newExpr = Operators.multiply x y 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -15*x*y*sin(x)