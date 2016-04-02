#Numbers.min

	val min : ax : Expression list ->  Expression


#####CompiledName: Min


####Описание
Возвращает минимальный элемент в списке выражений (Expression).
В случае передачи пустого списка как аргумента будет выброшено исключение


----------

####Пример

    Numbers.min [-2Q; 10Q; 0Q; 20Q/2 ]
    |> Infix.format
    |> printfn "%s"

####Вывод

	-2



