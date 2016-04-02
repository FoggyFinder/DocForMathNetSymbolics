#Structure.collectNumberValues

	val collectNumberValues: x : Expression -> MathNet.Numerics.BigRational list


#####CompiledName: CollectNumberValues


####Описание

Собирает все числа в выражении и возвращает результат в виде списка из чисел
типа BigRational (MathNet.Numerics) без повторений

----------

####Пример

    "pi*tan(y) + 2*sin(2*x)*cos(3*x+y)" 
    |> Infix.parseOrUndefined
    |> Structure.collectNumberValues
    |> List.iter(printfn "%A")

####Вывод

    2N
    3N

