#Structure.collectConstants

	val collectConstants: x : Expression -> Constant list


#####CompiledName: CollectConstants


####Описание

Собирает все константы из Expression и возвращает отдельные Expression без повторений.


----------

####Пример

	"pi + e*2*sin(x)" 
	|> Infix.parseOrUndefined
	|> Structure.collectConstants
	|> List.iter(printfn "%A")

####Вывод

	Constant E
	Constant Pi
