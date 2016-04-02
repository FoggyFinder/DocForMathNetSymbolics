#Polynomial.degreeMonomial

	val degreeMonomial:  symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: MonomialDegree


####Описание
Определяет степень монома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "3*w*x^2*y^3" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    Polynomial.degreeMonomial x expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод

	3*w*x^2*y^3
	2






