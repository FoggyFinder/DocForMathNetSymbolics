#Polynomial.leadingCoefficientDegree

	val leadingCoefficientDegree : symbol : Expression -> x : Expression -> Expression*Expression


#####CompiledName: LeadingCoefficientDegree


####Описание

Возвращает коэффициент и значение степени у полиномиального терма с максимальной степенью

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "3*x^5 - 2*x^3 - 4*x^2 + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    print expr
    
    expr
    |> Polynomial.leadingCoefficientDegree x
    |> fun (c,d) -> print c; print d
    

####Вывод

    1 - 4*x^2 - 2*x^3 + 3*x^5
    3
    5








