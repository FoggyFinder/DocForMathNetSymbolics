#Polynomial.coefficients

	val coefficients: symbol : Expression -> x : Expression ->  Expression[]


#####CompiledName: Coefficients


####Описание
Возвращает массив, состоящий из коэффициентов полинома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "3 + 4*x + 6*x*y + 12*x^2" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    Polynomial.coefficients x expr
    |> Seq.map(Infix.format)
    |> Seq.iter(printfn "%s")


####Вывод
    
    3
    4 + 6*y
    12

