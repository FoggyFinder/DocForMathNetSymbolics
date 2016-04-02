#Operators.productSeq

	val productSeq : xs : seq<Expression> -> Expression


#####CompiledName: productSeq


####Описание

Перемножает выражения в последовательности (включая списки и массивы) между собой

    
----------

####Пример

    let data = [| "4*x";"5*y";"7*x";"3*sin(x*y)" |]
    let listExpr = data |> Array.map(Infix.parseOrUndefined)
    let newExpr = listExpr |> Operators.productSeq
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

     420*x^2*y*sin(x*y)
