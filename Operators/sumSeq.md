#Operators.sumSeq

	val sumSeq : xs : seq<Expression> -> Expression


#####CompiledName: sumSeq


####Описание

Суммирует последовательность (включая списки и массивы) выражении 

    
----------

####Пример

    let data = [| "4*x";"5*y";"7*x";"3*sin(x*y)" |]
    let listExpr = data |> Array.map(Infix.parseOrUndefined)
    let newExpr = listExpr |> Operators.sumSeq
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    11*x + 5*y + 3*sin(x*y)