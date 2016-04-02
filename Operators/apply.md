#Operators.apply

	val apply : f : Function -> x : Expression ->  Expression


#####CompiledName: apply


####Описание

Применяет к выражению функцию, заданную через размеченное объединение Function
    
----------

####Пример
    
    let x = "-10" |> Infix.parseOrUndefined
    let func = Function.Abs
    let newExpr = Operators.apply func x
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    10


