#Polynomial.diophantineGcd

	val diophantineGcd : symbol : Expression -> u : Expression -> v : Expression -> w : Expression ->  Expression * Expression


#####CompiledName: DiophantineGcd


####Описание
Находит решение для линейного диофантового уравнения с двумя неизвестными
для заданной переменной (***symbol***)

    a*u + b*v = w

----------

####Пример
    
    
    let u = "3*x + 4" |> Infix.parseOrUndefined
    let v = "2*x^2 - x + 1" |> Infix.parseOrUndefined
    let w = "6*x^3 - 4*x^2 + x - 2" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    let a, b = Polynomial.diophantineGcd x u v w
    
    let print = Infix.format >> printfn "%s"
    
    printf "u: "
    print u
    printf "v: "
    print v
    printf "w: "
    print w
    
    printfn "Find a, b such that a*u + b*v = w"
    
    printf "a: "
    print a
    printf "b: "
    print b
    

####Вывод

    u: 4 + 3*x
    v: 1 - x + 2*x^2
    w: -2 + x - 4*x^2 + 6*x^3
    Find a, b such that a*u + b*v = w
    a: -24/53 - (11/53)*x
    b: -10/53 + 3*x






