#Polynomial.leadingCoefficient

	val leadingCoefficient : symbol : Expression -> x : Expression ->  Expression


#####CompiledName: LeadingCoefficient


####Описание

Возвращает коэффициент при старшей степени полинома.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "2*x^3 + 4*x^3*x - 2*x^2 + 5" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> SingleVariablePolynomial.leadingCoefficientSV x
    |> print
    

####Вывод
    
    5 - 2*x^2 + 2*x^3 + 4*x^4
    4
    
    







