#Evaluate.evaluate

	val evaluate : symbols : IDictionary<string, FloatingPoint> -> _arg1 : Expression -> FloatingPoint


#####CompiledName: Evaluate


####Описание
	
Проводит расчет значения выражения 

----------

####Пример

    let f = "x + x^2" |> Infix.parseOrUndefined
    
    f 
    |> Infix.format
    |> printfn "f(x) = %s" 
    
    let value x = Map.ofList ["x", FloatingPoint.Real x]
    
    [0.0..4.0]
    |> List.map(fun x -> x, x |> value |> (fun y -> Evaluate.evaluate y f))
    |> List.iter(fun (x,y) -> printfn "f(%f) = %A" x y)

####Вывод

    f(x) = x + x^2
    f(0.000000) = Real 0.0
    f(1.000000) = Real 2.0
    f(2.000000) = Real 6.0
    f(3.000000) = Real 12.0
    f(4.000000) = Real 20.0


