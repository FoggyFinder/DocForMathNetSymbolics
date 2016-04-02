#Evaluate.fmultiply

	val fmultiply : u : FloatingPoint -> v : FloatingPoint ->  FloatingPoint


#####CompiledName: fmultiply


####Описание
	
Перемножает два значения FloatingPoint

----------

####Пример

    let x = FloatingPoint.Real 10.0
    let y = FloatingPoint.Real 15.0
    
    Evaluate.fmultiply x y 
    |> printfn "%A * %A = %A" x y 

####Вывод

    Real 10.0 * Real 15.0 = Real 150.0

