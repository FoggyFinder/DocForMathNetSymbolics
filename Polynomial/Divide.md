#Polynomial.divide

	val divide :symbol : Expression -> u : Expression -> v : Expression -> Expression * Expression


#####CompiledName: Divide


####Описание
Евклидово деление многочленов. Возвращает кортеж с q и r и таких, что

    u = q*v + r
    
----------

####Пример
    
    
    let u = "x^2 - 5*x - 6" |> Infix.parseOrUndefined
    let v = "x + 1" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    
    let q, r = Polynomial.divide x u v
    
    let print = Infix.format >> printfn "%s"
    
    printf "u: "
    print u
    printf "v: "
    print v
    
    printfn "Find q, r such that u = q*v + r"
    
    printf "q: "
    print q
    printf "r: "
    print r
    

####Вывод
    
    u: -6 - 5*x + x^2
    v: 1 + x
    Find q, r such that u = q*v + r
    q: -6 + x
    r: 0







