#Operators.divide

	val divide : x : Expression -> y : Expression ->  Expression


#####CompiledName: divide


####Описание

Возвращает частное двух выражений
    
----------

####Пример
    
    let x = "-3*x" |> Infix.parseOrUndefined
    let y = "5*y*sin(x)" |> Infix.parseOrUndefined
    
    let newExpr = Operators.divide x y 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -((3/5)*x)/(y*sin(x))


