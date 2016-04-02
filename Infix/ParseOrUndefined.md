#Infix.parseOrUndefined

	val parseOrUndefined: infix: string -> Expression


#####CompiledName: ParseOrUndefined


####Описание
Проводит разбор математического выражения, которое задается
в виде строки. Возвращает дерево выражений (Expression). 
В случае ошибки входных данных вернет Undefined.

----------

####Пример

	let goodExample = "2*x + 3*y + cos(x*y*z)"
	let badExample = "2*x + 3*y + cos(x*y*z"

	goodExample
	|> Infix.parseOrUndefined |> Infix.print
	|> printfn "%s"

	badExample
	|> Infix.parseOrUndefined |> Infix.print
	|> printfn "%s"

####Вывод

	2*x + 3*y + cos(x*y*z)
	Undefined
