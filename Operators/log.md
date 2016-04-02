#Operators.ln 

	val log : basis : Expression -> x : Expression ->  Expression"


#####CompiledName: log


####Описание

Возвращает логарифм выражения с указанным основанием (***basic***) 
    
----------

####Пример
    
    let exp = "4*x" |> Infix.parseOrUndefined
    
    let newExpr = Operators.log 8Q exp 
    
    newExpr
    |> Infix.format
    |> printfn "%s"

####Вывод

    ln(4*x)/ln(8)


