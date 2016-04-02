#Operators.cot

	val cot : x : Expression ->  Expression


#####CompiledName: cot


####Описание

Возвращает котангенс заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.cot exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    1/tan(4*x)

