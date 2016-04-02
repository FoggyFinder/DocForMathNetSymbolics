#Operators.abs

	val abs: : _arg1 : Expression ->  Expression


#####CompiledName: abs


####Описание

Возвращает модуль выражения
    
----------

####Пример

    let expr = "-3*x" |> Infix.parseOrUndefined
    let newExpr = Operators.abs expr
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    |3*x|



