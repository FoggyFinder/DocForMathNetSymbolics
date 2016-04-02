#SingleVariablePolynomial.leadingCoefficientDegreeSV

	val leadingCoefficientDegreeSV : symbol : Expression -> x : Expression -> Expression*Expression


#####CompiledName: LeadingCoefficientDegree


####Описание

Возвращает коэффициент и значение степени у полиномиального терма с максимальной степенью

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "2*x^3 + x^3*x - 2*x^2 + 5" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> SingleVariablePolynomial.leadingCoefficientDegreeSV x
    |> fun (c,d) -> print c; print d
    
####Вывод
    
    5 - 2*x^2 + 2*x^3 + x^4
    1
    4
    








