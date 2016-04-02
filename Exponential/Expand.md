#Exponential.expand

	val expand : x : Expression ->  Expression


#####CompiledName: Expand


####Описание
	
"Разворачивает" математическое выражение с экспонентами на слагаемые

----------

####Пример

    let expr = "exp(2*x+y)/exp(x-y)" |> Infix.parseOrUndefined
    
    Exponential.expand expr
    |> Infix.format
    |> printfn "%s"


####Вывод

    exp(x)*exp(y)^2


