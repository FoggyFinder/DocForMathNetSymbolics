#Structure.collectIdentifiers

	val collectIdentifiers: x : Expression -> Expression list


#####CompiledName: CollectIdentifiers


####Описание

Собирает все идентификаторы в выражении и возвращает их в виде выражений без повторений

----------

####Пример

    "pi*tan(y) + sin(2*x)*cos(x+y) + sin(2*x)" 
    |> Infix.parseOrUndefined
    |> Structure.collectIdentifiers
    |> List.iter(Infix.print >> printfn "%A")

####Вывод

    "x"
    "y"


