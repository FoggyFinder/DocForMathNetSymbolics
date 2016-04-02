#NumericLiteralQ.FromOne

	val FromOne : unit ->  Expression


#####CompiledName: FromOne


####Описание
Функция, которая возвращает константу 1. Обертка над Expression.One.

----------

####Пример

    NumericLiteralQ.FromOne()
    |> Infix.format
    |> printfn "%s"

####Вывод

	1