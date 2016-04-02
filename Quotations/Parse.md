#Quotations.parse

	val parse: q : Quotations.Expr -> MathNet.Symbolics.Expression



#####CompiledName: Parse


####Описание

Конвертирует квотируемое (цитируемое) выражение из Quotations.Expr в Expression (MathNet.Symbolics)

----------

####Пример

	let qexpr = <@ fun x y -> (x + 2) * (y - 7) @>
	qexpr |> printfn "%A"

	let qsexpr = qexpr |> Quotations.parse
	qsexpr |> Infix.print |> printfn "%s"

####Вывод

	Lambda (x,
        Lambda (y,
                Call (None, op_Multiply,
                      [Call (None, op_Addition, [x, Value (2)]),
                       Call (None, op_Subtraction, [y, Value (7)])])))
	(2 + x)*(-7 + y)


