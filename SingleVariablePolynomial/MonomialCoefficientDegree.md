#SingleVariablePolynomial.coefficientDegreeMonomialSV

	val coefficientDegreeMonomialSV :symbol : Expression -> _arg1 : Expression -> Expression * Expression


#####CompiledName: MonomialCoefficientDegree


####Описание

Возвращает коэффициент и максимальную степень монома с одной переменной (***symbol***).

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "5*x^3" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr 
    
    expr
    |> SingleVariablePolynomial.coefficientDegreeMonomialSV x
    |> fun (c,d) -> print c; print d
    
####Вывод
    
    5*x^3
    5
    3
    
    
        





