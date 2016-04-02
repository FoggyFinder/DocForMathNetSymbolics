#Structure.operand

	val operand: i : Int32 -> _arg1 : Expression ->  Expression


#####CompiledName: Operand


####Описание

Возвращает ***i*** - ый операнд выражения (Expression)

----------

####Пример

    let str = "2*x^3 + 4*tan(x) + sin(x)*cos(y) - 5*z"
    let expr = str |> Infix.parseOrUndefined
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    let count = expr |> Structure.numberOfOperands
    {0..count - 1}
    |> Seq.map(fun x -> Structure.operand x expr)
    |> Seq.iteri(fun i x -> x |> Infix.format |> printfn "%i. %s" i)

####Вывод

    2*x^3 - 5*z + sin(x)*cos(y) + 4*tan(x)
    0. 2*x^3
    1. -5*z
    2. sin(x)*cos(y)
    3. 4*tan(x)

