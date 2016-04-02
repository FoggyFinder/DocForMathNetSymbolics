#Polynomial.collectTerms

	val collectTerms: symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: CollectTerms


####Описание
Собирает полиномиальные термы

----------

####Пример

    let expr = "3 + 4*x + 6*x*y + 12*x^2" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let x = symbol "x"
    
    Polynomial.collectTerms x expr
    |> Infix.format
    |> printfn "%s"


####Вывод
    
    3 + 4*x + 12*x^2 + 6*x*y
    3 + 12*x^2 + x*(4 + 6*y)


