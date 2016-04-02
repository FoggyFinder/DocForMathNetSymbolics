#SingleVariablePolynomial.isPolynomialSV

	val isPolynomialSV : symbol : Expression -> _arg1 : Expression ->  Boolean


#####CompiledName: IsPolynomial


####Описание

Проверяет, является ли выражение полиномом с одной переменной.

----------

####Пример
    
    let x = symbol "x"
    
    ["2*x*y";"x + 3*x^4";"x^2 + sin(x)"]
    |> List.map(Infix.parseOrUndefined >> SingleVariablePolynomial.isPolynomialSV x)
    |> List.iter(printfn "%b")
    

####Вывод
    
    false
    true
    false
    
    






