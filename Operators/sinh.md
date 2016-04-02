#Operators.sinh

	val sinh : x : Expression ->  Expression


#####CompiledName: sinh


####Описание

Возвращает гиперболический синус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.sinh exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    sinh(4*x)


