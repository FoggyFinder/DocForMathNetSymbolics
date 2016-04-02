#Evaluate.fapply

	val fapply : f : Function -> u : FloatingPoint ->  FloatingPoint


#####CompiledName: fapply


####Описание

Применяет функцию, заданную размеченным объединением **Function**
к значению **FloatingPoint**
 
----------

####Пример
    
    let f = Function.Cos
    let y = FloatingPoint.Real 0.0
    
    Evaluate.fapply f y 
    |> printfn "%A(%A) = %A" f y 

####Вывод

    Cos(Real 0.0) = Real 1.0

