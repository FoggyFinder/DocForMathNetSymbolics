#Operators.add

	val add: x : Expression -> y : Expression ->  Expression


#####CompiledName: add


####Описание

    Возвращает сумму двух выражений
    
----------

####Пример

    let x = "-3*x" |> Infix.parseOrUndefined
    let y = "5*y*sin(x)" |> Infix.parseOrUndefined
    
    let newExpr = Operators.add x y 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -3*x + 5*y*sin(x)



