#Polynomial.coefficientMonomial

	val coefficientMonomial: symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: MonomialCoefficient


####Описание
Возвращает коэффициент монома для заданной переменной (***symbol***)

----------

####Пример
    
    let expr = "5*x*y*z" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let x = symbol "x"
    
    Polynomial.coefficientMonomial x expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    5*x*y*z
    5*y*z





