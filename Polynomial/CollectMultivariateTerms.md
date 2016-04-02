#Polynomial.collectTermsMV

	val collectTermsMV: symbols : HashSet<Expression> -> _arg1 : Expression ->  Expression


#####CompiledName: CollectMultivariateTerms


####Описание
Собирает полиномиальные термы, относительно всех символов, заданных через
множество (System.Collections.Generic.HashSet)

----------

####Пример

    let expr = "3*x*y + 4*x - 3*z*x - 4*y*z + 5*y" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let hs = new HashSet<Expression>([| symbol "x"; symbol "y" |])
    
    Polynomial.collectTermsMV hs expr
    |> Infix.format
    |> printfn "%s"


####Вывод
    
    4*x + 5*y + 3*x*y - 3*x*z - 4*y*z
    3*x*y + y*(5 - 4*z) + x*(4 - 3*z)



