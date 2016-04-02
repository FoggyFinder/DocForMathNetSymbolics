#Polynomial.isPolynomialMV

	val isPolynomialMV : symbols : HashSet<Expression> -> _arg1 : Expression ->  Expression


#####CompiledName: IsMultivariatePolynomial


####Описание

Проверяет, является ли выражение полиномом для заданного множества символов.

----------

####Пример
    
    let hs = HashSet<Expression>([symbol "x"; symbol "y"])
    
    ["2*x*y";"x + y^2";"x^2 + sin(x)*y"]
    |> List.map(Infix.parseOrUndefined >> Polynomial.isPolynomialMV hs)
    |> List.iter(printfn "%b")
    
####Вывод
    
    true
    true
    false
