#Structure.collectNumbers

	val collectNumbers: x : Expression -> Expression list


#####CompiledName: CollectNumbers


####Описание

Собирает все числа в выражении и возвращает результат в виде выражений без повторений

----------

####Пример

    "pi*tan(y) + 2*sin(2*x)*cos(3*x+y)" 
    |> Infix.parseOrUndefined
    |> Structure.collectNumbers
    |> List.iter(Infix.print >> printfn "%A")

####Вывод

    "2"
    "3"


