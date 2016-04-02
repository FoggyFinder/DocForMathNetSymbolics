#Numbers.max

	val max : ax : Expression list ->  Expression


#####CompiledName: Max


####Описание
Возвращает максимальный элемент в списке выражений (Expression).
В случае попытки узнать максимальный элемент пустого списка будет выброшено исключение


----------

####Пример

    Numbers.max [-2Q; 10Q; 0Q; 20Q/2 ]
    |> Infix.format
    |> printfn "%s"

####Вывод

	10



