#Polynomial.commonMonomialFactors

	val commonMonomialFactors : xs : Expression list ->  Expression


#####CompiledName: CommonMonomialFactors


####Описание
Находит общий множитель для списка мономов.

----------

####Пример
    
    let expr = ["5*x*y*z" ; "3*w*x*y^3"] |> List.map(Infix.parseOrUndefined)
    
    expr
    |> List.iter(Infix.format >> printfn "%s")
    
    Polynomial.commonMonomialFactors expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    5*x*y*z
    3*w*x*y^3
    x*y





