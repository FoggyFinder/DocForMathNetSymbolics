#Operators.sum

	val sum : xs : Expression list -> Expression


#####CompiledName: sum


####Описание

Суммирует выражения, записанные в списке
    
----------

####Пример

    let data = ["4*x";"5*y";"7*x";"3*sin(x*y)"]
    let listExpr = data |> List.map(Infix.parseOrUndefined)
    let newExpr = listExpr |> Operators.sum
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    11*x + 5*y + 3*sin(x*y)

