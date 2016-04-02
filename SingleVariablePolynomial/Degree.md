#SingleVariablePolynomial.degreeSV

	val degreeSV: symbol : Expression -> x : Expression ->  Expression


#####CompiledName: Degree


####Описание
Определяет степень полинома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "4*x + 8*x^3" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    SingleVariablePolynomial.degreeSV x expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    3
    



