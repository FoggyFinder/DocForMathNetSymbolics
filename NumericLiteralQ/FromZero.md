#NumericLiteralQ.FromZero

	val FromZero : unit ->  Expression


#####CompiledName: FromZero


####Описание
Функция, которая возвращает константу 0. Обертка над Expression.Zero.

----------

####Пример

    NumericLiteralQ.FromZero()
    |> Infix.format
    |> printfn "%s"

####Вывод

	0