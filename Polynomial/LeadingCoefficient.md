#Polynomial.leadingCoefficient

	val leadingCoefficient : symbol : Expression -> x : Expression ->  Expression


#####CompiledName: LeadingCoefficient


####Описание

Возвращает коэффициент при старшей степени полинома.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "3*x^5 - 2*x^3 - 4*x^2 + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> Polynomial.leadingCoefficient x
    |> print
    

####Вывод
    
    1 - 4*x^2 - 2*x^3 + 3*x^5
    3
    








