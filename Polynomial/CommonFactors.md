#Polynomial.commonFactors

	val commonFactors: x : Expression ->  Expression


#####CompiledName: CommonFactors


####Описание
Находит общий множитель полинома

----------

####Пример
    
    let expr = "4*x*y - 8*x*y*z" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    Polynomial.commonFactors expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    4*x*y - 8*x*y*z
    4*x*y




