#Operators.ln 

	val ln  : x : Expression ->  Expression


#####CompiledName: ln


####Описание

Возвращает натуральный логарифм от заданного выражения
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.ln exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    ln(4*x)


