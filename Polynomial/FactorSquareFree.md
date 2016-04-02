#Polynomial.factorSquareFree

	val factorSquareFree : symbol : Expression -> x : Expression ->  Expression


#####CompiledName: FactorSquareFree


####Описание

pulls out any multiple factors in a polynomial.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "x^5 - x^3 - x^2 + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> Polynomial.factorSquareFree x
    |> print
    

####Вывод
    
    1 - x^2 - x^3 + x^5
    (-1 + x)^2*(1 + 2*x + 2*x^2 + x^3)








