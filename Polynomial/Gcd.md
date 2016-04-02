#Polynomial.gcd

	val gcd : symbol : Expression -> u : Expression -> v : Expression ->  Expression


#####CompiledName: Gcd


####Описание
Возвращает наибольший общий делитель для полиномов
    
----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "x^2 - 5*x - 6" |> Infix.parseOrUndefined
    let v = "x^2 - 3*x - 4" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    let gcd = Polynomial.gcd x u v
    
    printf "u: "
    print u
    printf "v: "
    print v
    printf "gcd: "
    print gcd
    

####Вывод
    
    u: -6 - 5*x + x^2
    v: -4 - 3*x + x^2
    gcd: 1 + x







