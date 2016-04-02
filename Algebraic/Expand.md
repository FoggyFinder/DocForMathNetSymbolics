#Algebraic.expand

	val expand : _arg1 : Expression ->  Expression


#####CompiledName: Expand


####Описание
	
"Разворачивает" математическое выражение на слагаемые

----------

####Пример

    let expr = "3*(x+y)*(x+1)*(y+3)" |> Infix.parseOrUndefined
    
    Algebraic.expand expr
    |> Infix.format
    |> printfn "%s"

####Вывод

    9*x + 9*x^2 + 9*y + 12*x*y + 3*x^2*y + 3*y^2 + 3*x*y^2




