#Polynomial.totalDegree

	val totalDegree : x : Expression ->  Expression


#####CompiledName: TotalDegree


####Описание

Возвращает степень полинома, для всех переменных, которые в нем встречаются

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "2 + 3*x - 4*x^2 + 5*a*x^3" |> Infix.parseOrUndefined
    
    print expr
    
    expr
    |> Polynomial.totalDegree
    |> print
    

####Вывод
    
    2 + 3*x - 4*x^2 + 5*a*x^3
    4
    
        







