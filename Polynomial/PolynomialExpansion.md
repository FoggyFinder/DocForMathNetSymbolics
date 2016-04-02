#Polynomial.polynomialExpansion

	val polynomialExpansion : symbol : Expression -> t : Expression -> u : Expression -> v : Expression ->  Expression


#####CompiledName: PolynomialExpansion


####Описание

Проводит замену переменной

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "2*x^2-x-10" |> Infix.parseOrUndefined
    let v = "x+1" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    let y = symbol "y"
    
    printf "u: "
    print u
    
    printf "v: "
    print v
    
    Polynomial.polynomialExpansion x y u v
    |> print
    
####Вывод
    
    u: -10 - x + 2*x^2
    v: 1 + x
    -7 - 5*y + 2*y^2
    
    
    



