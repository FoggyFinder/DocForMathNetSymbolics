#Polynomial.isMonomial

	val isMonomial : symbol : Expression -> _arg1 : Expression ->  Boolean


#####CompiledName: IsMonomial


####Описание

Проверяет, является ли выражение мономом.

----------

####Пример

    let x = symbol "x"
    
    ["2*x*y";"(x^2 + 4)*(x^3+3)"]
    |> List.map(Infix.parseOrUndefined >> Polynomial.isMonomial x)
    |> List.iter(printfn "%b")

####Вывод
    
    true
    false







