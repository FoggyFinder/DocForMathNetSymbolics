#Operators.sin

	val sin : _arg1 : Expression ->  Expression


#####CompiledName: sin


####Описание

Возвращает синус заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.sin exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    sin(4*x)

