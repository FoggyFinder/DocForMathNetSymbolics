#Polynomial.variables

	val variables : x : Expression ->  HashSet<Expression>


#####CompiledName: Variables


####Описание

Возвращает переменные полинома

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "2 + 3*x - 4*x^2 + 5*a*x^3" |> Infix.parseOrUndefined
    
    print expr
    
    expr
    |> Polynomial.variables
    |> Seq.iter(print)
    
    

####Вывод
    
    2 + 3*x - 4*x^2 + 5*a*x^3
    x
    a
    
    







