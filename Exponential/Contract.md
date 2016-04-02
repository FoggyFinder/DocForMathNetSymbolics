#Exponential.contract

	val contract : x : Expression ->  Expression


#####CompiledName: Contract


####Описание
	
"Сокращает" математическое выражение с экспонентами

----------

####Пример

    let expr = "exp(2*x+y)/exp(x-y)" |> Infix.parseOrUndefined
    
    expr
    |> Exponential.contract
    |> Infix.format
    |> printfn "%s"



####Вывод

    exp(x + 2*y)
