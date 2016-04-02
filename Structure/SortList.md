#Structure.sortList

	val sortList: list : Expression list ->  Expression list 


#####CompiledName: SortList


####Описание

Сортирует список выражений 

----------

####Пример

    "pi*tan(y+a) + 2*sin(2*x)*cos(3*x+y) +c/z"
    |> Infix.parseOrUndefined
    |> Structure.collectIdentifiers
    |> Structure.sortList
    |> List.iter(Infix.print >> printfn "%s")

####Вывод

    a
    c
    x
    y
    z

