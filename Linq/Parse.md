#Linq.parse

	val parse: q: Linq.Expressions.Expression -> Expression


#####CompiledName: Parse


####Описание
Конвертирует Expression из System.Linq.Expressions в
Expression (MathNet.Symbolics)

----------

####Пример

	type LExpr = System.Linq.Expressions.Expression

	//(x + 2) * (y - 7)
	let lexpr = LExpr.Multiply(
                	LExpr.Add(LExpr.Variable(typeof<int>,"x"), LExpr.Constant(2)),
                	LExpr.Subtract(LExpr.Variable(typeof<int>,"y"),LExpr.Constant(7)))
           
	lexpr |> printfn "%O"

	let sexpr = lexpr |> Linq.parse
	sexpr |> Infix.print |> printfn "%s"

####Вывод

	((x + 2) * (y - 7))
	(2 + x)*(-7 + y)


