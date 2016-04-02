#Algebraic.factors

	val factors : _arg1 : Expression -> Expression list


#####CompiledName: Factors


####Описание
	
Разбивает математическое выражение на множители

----------

####Пример

    let expr = "1/5*sin(x)*(x+2)*cos(3*t)" |> Infix.parseOrUndefined
    
    Algebraic.factors expr
    |> List.map(Infix.format)
    |> List.iter(printfn "%s")


####Вывод

    1/5
    2 + x
    sin(x)
    cos(3*t)


