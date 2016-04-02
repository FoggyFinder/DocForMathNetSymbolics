#Evaluate.fadd

	val fadd : u : FloatingPoint -> v : FloatingPoint ->  FloatingPoint


#####CompiledName: fadd


####Описание
	
Складывает два значения FloatingPoint

----------

####Пример

    let x = FloatingPoint.Real 10.0
    let y = FloatingPoint.Real 15.0
    
    Evaluate.fadd x y 
    |> printfn "%A + %A = %A" x y 

####Вывод

    Real 10.0 + Real 15.0 = Real 25.0



