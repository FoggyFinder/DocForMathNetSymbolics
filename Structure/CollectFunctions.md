#Structure.collectFunctions

	val collectFunctions: x : Expression ->  Expression list


#####CompiledName: CollectFunctions


####Описание

Собирает все функции в выражении и возвращает результат без повторений

----------

####Пример

    "pi*tan(y) + sin(2*x)*cos(x+y) + sin(2*x)" 
    |> Infix.parseOrUndefined
    |> Structure.collectFunctions
    |> List.iter(Infix.print >> printfn "%s")

####Вывод

    sin(2*x)
    cos(x + y)
    tan(y)
