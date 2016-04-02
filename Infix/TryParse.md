#Infix.tryParse

	val tryParse: infix: String -> Expression option


#####CompiledName: TryParse


####Описание

Преобразует математическое выражение в виде строки в тип Expression option

----------

####Пример

	let goodExample = "2*x + 3*y + cos(x*y*z)"
	let badExample = "2*x + 3*y + cos(x*y*z"

	let printWithOption result = 
    	match result with
    	| Some str -> str |> Infix.print |> printfn "%s"
    	| None -> printfn "Ошибка при разборе"

	goodExample |> Infix.tryParse |> printWithOption
	badExample  |> Infix.tryParse |> printWithOption

####Вывод

	2*x + 3*y + cos(x*y*z)
	Ошибка при разборе