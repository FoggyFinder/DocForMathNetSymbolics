#Structure.collectIdentifierSymbols

	val collectIdentifierSymbols: x : Expression -> Symbol list


#####CompiledName: CollectIdentifierSymbols


####Описание

Собирает все идентификаторы в выражении и возвращает символы без повторений

----------

####Пример

    "pi*tan(y) + sin(2*x)*cos(x+y) + sin(2*x)" 
    |> Infix.parseOrUndefined
    |> Structure.collectIdentifierSymbols
    |> List.iter(printfn "%A")

####Вывод

    Symbol "x"
    Symbol "y"
