#Infix.parse

	val parse: infix: string -> ParseResult


#####CompiledName: Parse


####Описание
Преобразует математическое выражение в виде строки в тип ParseResult.

----------

####Пример

	let goodExample = "2*x + 3*y + cos(x*y*z)"
	let badExample = "2*x + 3*y + cos(x*y*z"

	let printWithParseResult result = 
    	match result with
    	| ParseFailure str -> str |> printfn "%s"
    	| ParsedExpression exp -> exp |> Infix.print |> printfn "%s"

	goodExample |> Infix.parse |> printWithParseResult
	badExample  |> Infix.parse |> printWithParseResult

#####Вывод

	2*x + 3*y + cos(x*y*z)
	Error in Ln: 1 Col: 16
	2*x + 3*y + cos(x*y*z
               ^
	Expecting: end of input or infix operator

