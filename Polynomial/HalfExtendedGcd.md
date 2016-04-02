#Polynomial.halfExtendedGcd

	val halfExtendedGcd : symbol : Expression -> u : Expression -> v : Expression ->  Expression


#####CompiledName: HalfExtendedGcd


####Описание
Returns a tuple with the gcd and a such that

     a*u = gcd (mod v)
    
----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "x^4 - 2*x^3 - 6*x^2 + 12*x + 15 " |> Infix.parseOrUndefined
    let v = "x^3 + x^2 - 4*x - 4" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    
    let gcd, a = Polynomial.halfExtendedGcd x u v
    
    printf "u: "
    print u
    printf "v: "
    print v
    printf "gcd: "
    print gcd
    printf "a: "
    print a
    

####Вывод
    
    u: 15 + 12*x - 6*x^2 - 2*x^3 + x^4
    v: -4 - 4*x + x^2 + x^3
    gcd: 1 + x
    a: 3/5 - (1/5)*x
    






