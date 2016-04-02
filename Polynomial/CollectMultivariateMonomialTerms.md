#Polynomial.collectTermsMonomialMV

	val collectTermsMonomialMV: symbols : HashSet<Expression> -> _arg1 : Expression -> Expression * Expression


#####CompiledName: CollectMultivariateMonomialTerms


####Описание
Собирает коэффициенты монома для переменных (***symbol***).
Результат - кортеж из двух элементов. Первый - часть без указанных символов.
Второй - сами переменные

----------

####Пример
    
    let expr = "5*x*y*z" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let hs = HashSet<Expression>([symbol "x"; symbol "y"])
    
    Polynomial.collectTermsMonomialMV hs expr
    |> fun (x,y) -> Infix.format x, Infix.format y
    |> printfn "%A"

    

####Вывод
    
    5*x*y*z
    ("5*z", "x*y")






