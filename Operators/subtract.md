#Operators.subtract

	val subtract: x : Expression -> y : Expression ->  Expression


#####CompiledName: subtract


####Описание

Вычитает выражение ***y*** из выражения ***x***
    
----------

####Пример

    let x = "-3*x" |> Infix.parseOrUndefined
    let y = "5*y*sin(x)" |> Infix.parseOrUndefined
    
    let newExpr = Operators.subtract x y 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -3*x - 5*y*sin(x)




