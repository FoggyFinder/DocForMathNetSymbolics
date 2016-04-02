#Evaluate.fnormalize

	val fnormalize : _arg1 : FloatingPoint ->  FloatingPoint


#####CompiledName: fnormalize


####Описание
	
"Нормализует" значение FloatingPoint

----------

####Пример

    let value = 
    	System.Double.NegativeInfinity
    	|> FloatingPoint.Real
    
    value
    |> printfn "%A"
    
    value
    |> Evaluate.fnormalize
    |> printfn "%A"

####Вывод

    Real -infinity
    NegInf




