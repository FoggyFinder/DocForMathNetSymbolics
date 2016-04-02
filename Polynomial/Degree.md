#Polynomial.degree

	val degree: symbol : Expression -> x : Expression ->  Expression


#####CompiledName: Degree


####Описание
Определяет степень полинома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "4*x*y + 8*x^3" |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let x = symbol "x"
    
    Polynomial.degree x expr
    |> Infix.format
    |> printfn "%s"
    

####Вывод

    8*x^3 + 4*x*y
    3





