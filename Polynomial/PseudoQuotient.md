#Polynomial.pseudoQuot

	val pseudoQuot : symbol : Expression -> u : Expression -> v : Expression ->  Expression


#####CompiledName: PseudoQuotient


####Описание

Возвращает псевдо частное при деления двух полиномов для заданной переменной (***symbol***)

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "3*x^3 + x^2 + x + 5" |> Infix.parseOrUndefined
    let v = "5*x^2 - 3*x + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    printf "u: "
    print u
    
    printf "v: "
    print v
    
    printf "r: "
    Polynomial.pseudoQuot x u v 
    |> print

####Вывод
    
    u: 5 + x + x^2 + 3*x^3
    v: 1 - 3*x + 5*x^2
    r: 14 + 15*x
    
    
    
    






