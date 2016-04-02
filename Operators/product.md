#Operators.product

	val product : xs : Expression list -> Expression


#####CompiledName: product


####Описание

Перемножает выражения, записанные в списке
    
----------

####Пример

    let data = [ "4*x";"5*y";"7*x";"3*sin(x*y)" ]
    let listExpr = data |> List.map(Infix.parseOrUndefined)
    let newExpr = listExpr |> Operators.product
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    420*x^2*y*sin(x*y)


