#Polynomial.collectTermsMonomial

	val coefficientMonomial: symbol : Expression -> _arg1 : Expression ->  Expression * Expression


#####CompiledName: CollectMonomialTerms


####Описание
Собирает коэффициенты монома для переменной (***symbol***).
Результат - кортеж из двух элементов. Первый - часть без заданного символа. Второй - сам символ.

----------

####Пример
    
    let expr = "5*x*y*z" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let x = symbol "x"
    
    Polynomial.collectTermsMonomial x expr
    |> fun (x,y) -> Infix.format x, Infix.format y
    |> printfn "%A"
    

####Вывод
    
    5*x*y*z
    ("5*y*z", "x")





