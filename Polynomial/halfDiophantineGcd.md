#Polynomial.halfDiophantineGcd

	val halfDiophantineGcd : symbol : Expression -> u : Expression -> v : Expression ->  Expression


#####CompiledName: halfDiophantineGcd


####Описание
Returns a, such that
    
     a*u = w (mod v)
    
----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "x^4 - 2*x^3 - 6*x^2 + 12*x + 15 " |> Infix.parseOrUndefined
    let v = "x^3 + x^2 - 4*x - 4" |> Infix.parseOrUndefined
    let w = "x^2 - 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    let a = Polynomial.halfDiophantineGcd x u v w
    
    printf "u: "
    print u
    printf "v: "
    print v
    printf "w: "
    print v
    printf "a: "
    print a
    

####Вывод
    
    u: 15 + 12*x - 6*x^2 - 2*x^3 + x^4
    v: -4 - 4*x + x^2 + x^3
    w: -4 - 4*x + x^2 + x^3
    a: -3/5 + (4/5)*x - (1/5)*x^2







