#Algebraic.summands

	val summands : _arg1 : Expression -> Expression list


#####CompiledName: Summands


####Описание
	
Разбивает математическое выражение на слагаемые

----------

####Пример

    let expr = "3*x + y^4 + (x+2)*cos(3*t)" |> Infix.parseOrUndefined
    
    Algebraic.summands expr
    |> List.map(Infix.format)
    |> List.iter(printfn "%s")

####Вывод

    3*x
    y^4
    (2 + x)*cos(3*t)

