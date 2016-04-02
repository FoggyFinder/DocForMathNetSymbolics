#Structure.collect

	val collect: chooser : (Expression -> 'a option) -> x : Expression -> 'a list


#####CompiledName: Collect


####Описание

Применяет заданную функцию к дереву выражений и возвращает результат
для каждого узла, в котором функция возвращает Some с некоторым значением.

Подвыражений выражения рассматриваются только, если функция возвращает
None при применении к выражению.

Результаты возвращаются в виде списка в обратном порядке углубления.

----------

####Пример

	let getSymbol(Symbol(z)) = z

	let getIdentifier = 
    	function
    	| Identifier x -> x |> getSymbol |> Some
    	| _ -> None

	let expr = "2*x + 3*y + cos(a^y)" |> Infix.parseOrUndefined

	expr
	|> Structure.collect getIdentifier
	|> Seq.distinct
	|> Seq.iter(printfn "%A")

####Вывод

	"y"
	"a"
	"x"
