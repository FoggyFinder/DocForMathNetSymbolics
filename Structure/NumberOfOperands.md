#Structure.numberOfOperands

	val numberOfOperands: _arg1 : Expression ->  Int32


#####CompiledName: NumberOfOperands


####Описание

Возвращает количество операндов в выражении (Expression)

----------

####Пример

    let str = "2*x^3 + 4*tan(x) + sin(x)*cos(y) - 5*z"
    let expr = str |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    expr
    |> Structure.numberOfOperands
    |> printfn "%i"


####Вывод

    2*x^3 - 5*z + sin(x)*cos(y) + 4*tan(x)
    4

