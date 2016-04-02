#SingleVariablePolynomial.coefficientsSV

	val coefficientsSV: symbol : Expression -> x : Expression ->  Expression[]


#####CompiledName: Coefficients


####Описание
Возвращает массив, состоящий из коэффициентов полинома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "3 + 4*x + 12*x^2" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    SingleVariablePolynomial.coefficientsSV x expr
    |> Seq.map(Infix.format)
    |> Seq.iter(printfn "%s")
    
    
####Вывод
    
    3
    4
    12
    
