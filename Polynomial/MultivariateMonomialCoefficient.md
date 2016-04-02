#Polynomial.coefficientMonomialMV

	val coefficientMonomialMV : symbols : HashSet<Expression> -> _arg1 : Expression -> Expression


#####CompiledName: MultivariateMonomialCoefficient


####Описание

Возвращает коэффициент монома для заданного множества символов.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "5*a*y*x^3" |> Infix.parseOrUndefined
    let hs = HashSet<Expression>([symbol "x"; symbol "a"])
    
    expr
    |> Polynomial.coefficientMonomialMV hs
    |> print
    
####Вывод
    
    5*y
    
    



