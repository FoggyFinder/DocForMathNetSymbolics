#Polynomial.degreeMonomialMV

	val degreeMonomialMV : symbols : HashSet<Expression> -> _arg1 : Expression ->  Expression


#####CompiledName: MultivariateMonomialDegree


####Описание
Находит степень монома для заданного множества символов ***symbol***
(System.Collections.Generic.HashSet)

----------

####Пример
    
    
    let expr = "5*x^3*y*w" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let hs = HashSet<Expression>([symbol "x"; symbol "y"])
    
    Polynomial.degreeMonomialMV hs expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод

    5*w*x^3*y
    4






