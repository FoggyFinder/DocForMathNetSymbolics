#SingleVariablePolynomial.coefficientMonomialSV

	val coefficientMonomialSV: symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: MonomialCoefficient


####Описание
Возвращает коэффициент монома с одной переменной (***symbol***)

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "5*x*x" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    SingleVariablePolynomial.coefficientMonomialSV x expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    5*x^2
    5
    
    


