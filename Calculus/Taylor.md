#Calculus.taylor

	val taylor : k : Int32 -> symbol : Expression -> value : Expression -> expression : Expression ->  Expression


#####CompiledName: Taylor


####Описание
	
Позволяет разложить функцию (***expression***) в ряд Тейлора в окрестности точки (***value***),
 оставляя указанное (***k***) число слагаемых для заданного символа (***symbol***)

----------

####Пример

    let expr = "(x-2)*(x+3)" |> Infix.parseOrUndefined
    
    let x = symbol "x"
    let value = 4Q
    let count = 3
    
    Calculus.taylor count x value expr
    |> Infix.format
    |> printfn "%s"
    
####Вывод

    -6 + x + x^2





