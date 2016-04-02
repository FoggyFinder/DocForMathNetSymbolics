#Operators.tanh

	val tanh : x : Expression ->  Expression


#####CompiledName: tanh


####Описание

Возвращает гиперболический тангенс выражения
    
----------

####Пример

    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.tanh exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    tanh(4*x)

