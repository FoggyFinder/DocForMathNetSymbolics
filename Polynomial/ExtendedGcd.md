#Polynomial.extendedGcd

	val extendedGcd : symbol : Expression -> u : Expression -> v : Expression -> Expression * Expression * Expression 


#####CompiledName: ExtendedGcd


####Описание
Возвращает кортеж из трех элементов gcd, a, b таких, что:
    
    a*u + b*v = gcd(u,v)
    
----------

####Пример
    
    let u = "x^2 - 5*x - 6" |> Infix.parseOrUndefined
    let v = "x^2 - 3*x - 4" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    
    let gsd, a, b = Polynomial.extendedGcd x u v
    
    let print = Infix.format >> printfn "%s"
    
    printf "u: "
    print u
    printf "v: "
    print v
    
    printfn "Find gcd, a, b such that a*u + b*v = gcd(u,v)"
    
    printf "gsd: "
    print gsd
    printf "a: "
    print a
    printf "b: "
    print b
    

####Вывод

    u: -6 - 5*x + x^2
    v: -4 - 3*x + x^2
    Find gcd, a, b such that a*u + b*v = gcd(u,v)
    gsd: 1 + x
    a: -1/2
    b: 1/2







