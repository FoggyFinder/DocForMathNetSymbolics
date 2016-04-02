#Evaluate.fpower

	val fpower : u : FloatingPoint -> v : FloatingPoint ->  FloatingPoint


#####CompiledName: fpower


####Описание
	
Возводит ***u*** в степень ***v***

----------

####Пример

    let x = FloatingPoint.Real 3.0
    let y = FloatingPoint.Real 4.0
    
    Evaluate.fpower x y 
    |> printfn "%A ^ %A = %A" x y 

####Вывод

    Real 3.0 ^ Real 4.0 = Real 81.0


