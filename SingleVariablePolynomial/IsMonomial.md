#SingleVariablePolynomial.isMonomialSV

	val isMonomialSV : symbol : Expression -> _arg1 : Expression ->  Boolean


#####CompiledName: IsMonomial


####Описание

Проверяет, является ли выражение мономом с одной переменной.

----------

####Пример
    
    let x = symbol "x"
    
    ["2*x*y";"2*x^3"]
    |> List.map(Infix.parseOrUndefined >> SingleVariablePolynomial.isMonomialSV x)
    |> List.iter(printfn "%b")
    
####Вывод
    
    false
    true
    
    





