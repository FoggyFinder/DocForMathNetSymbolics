#Structure.collectConstantValues

	val collectConstantValues: x: (string -> Expression list)


#####CompiledName: CollectConstantValues


####Описание

Собирает все константы в выражении (Expression) и возвращает их значения без повторений

----------

####Пример

	"pi + e*2*sin(x)" 
	|> Infix.parseOrUndefined
	|> Structure.collectConstantValues
	|> List.iter(printfn "%A")

####Вывод

	E
	Pi

