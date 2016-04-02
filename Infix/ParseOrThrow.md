#Infix.parseOrThrow


	val parse: infix: string -> Expression


#####CompiledName: ParseOrThrow


####Описание

Пытается провести разбор математического выражения в виде строки.
В случае успеха возвращает Expression, в противном случае - выбрасывает исключение.


----------

####Пример

	let goodExample = "2*x + 3*y + cos(x*y*z)"
	let badExample = "2*x + 3*y + cos(x*y*z"

	let printExpr expr = 
    	try 
        	expr |> Infix.parseOrThrow |> Infix.print|> printfn "%s"
    	with
        	| _ as ex -> ex.Message |> printfn "%s" 

	goodExample |> printExpr
	badExample |> printExpr

#####Вывод

	2*x + 3*y + cos(x*y*z)
	Error in Ln: 1 Col: 16
	2*x + 3*y + cos(x*y*z
               ^
	Expecting: end of input or infix operator