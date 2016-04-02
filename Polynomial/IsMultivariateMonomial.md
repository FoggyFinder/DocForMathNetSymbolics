#Polynomial.isMonomialMV

	val isMonomialMV : symbols : HashSet<Expression> -> _arg1 : Expression ->  Expression


#####CompiledName: IsMultivariateMonomial


####Описание

Проверяет, является ли выражение мономом для заданного множества символов.

----------

####Пример
    
    let hs = HashSet<Expression>([symbol "x"; symbol "y"])
    
    ["2*x*y";"x + y^2"]
    |> List.map(Infix.parseOrUndefined >> Polynomial.isMonomialMV hs)
    |> List.iter(printfn "%b")
    
####Вывод
    
    true
    false
