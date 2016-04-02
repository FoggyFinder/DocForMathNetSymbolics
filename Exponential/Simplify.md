#Exponential.simplify

	val simplify : x : Expression ->  Expression


#####CompiledName: Simplify


####Описание
	
Упрощает математическое выражение с экспонентами

----------

####Пример

    let expr = "exp(2*x+y)/exp(x-y)" |> Infix.parseOrUndefined
    
    expr
    |> Exponential.expand 
    |> Exponential.simplify
    |> Infix.format
    |> printfn "%s"
    

####Вывод

    exp(x + 2*y)
