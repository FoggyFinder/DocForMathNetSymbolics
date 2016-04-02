#Structure.collectDistinct

	val collectDistinct: chooser : (Expression -> 'a option) -> x : Expression -> 'a list 


#####CompiledName: CollectDistinct


####Описание

Действует аналогично функции [collect](Collect.html), но возвращает 
выражения без повторений.

----------

####Пример

	let getSymbol(Symbol(z)) = z

	let getIdentifier = 
    	function
    	| Identifier x -> x |> getSymbol |> Some
    	| _ -> None

	"pi + e*2*sin(x+y) + x*y*z^3" 
	|> Infix.parseOrUndefined
	|> Structure.collectDistinct getIdentifier
	|> List.iter(printfn "%A")


####Вывод

	"y"
	"x"
	"z"
