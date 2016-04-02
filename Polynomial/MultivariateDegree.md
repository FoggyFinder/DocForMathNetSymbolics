#Polynomial.degreeMV 

	val degreeMV : symbols : HashSet<Expression> -> x : Expression ->  Expression


#####CompiledName: MultivariateDegree


####Описание
Определяет степень полинома для заданного множества символов ***symbol***
(System.Collections.Generic.HashSet)

----------

####Пример
    
    let expr = "5*x*y + 8*x^3*y" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let hs = HashSet<Expression>([symbol "x"; symbol "y"])
    
    Polynomial.degreeMV hs expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    5*x*y + 8*x^3*y
    4






