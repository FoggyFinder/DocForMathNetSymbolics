#Polynomial.isPolynomial

	val isPolynomial : symbol : Expression -> _arg1 : Expression ->  Boolean


#####CompiledName: IsPolynomial


####Описание

Проверяет, является ли выражение полиномом.

----------

####Пример
    
    let x = symbol "x"
    
    ["2*x*y";"x + y^2";"x^2 + sin(x)*y"]
    |> List.map(Infix.parseOrUndefined >> Polynomial.isPolynomial x)
    |> List.iter(printfn "%b")

####Вывод
    
    true
    true
    false








