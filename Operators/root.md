#Operators.root

	val root : n : Expression -> x : Expression ->  Expression


#####CompiledName: root


####Описание

Возвращает корень ***n*** - ой степени из заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    let n = 4Q
    let newExpr = Operators.root n exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    (4*x)^(1/4)

