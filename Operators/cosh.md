#Operators.cosh

	val cosh : x : Expression ->  Expression


#####CompiledName: cosh


####Описание

Возвращает гиперболический косинус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.cosh exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    cosh(4*x)

