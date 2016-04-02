#NumericLiteralQ.FromInt64

	val FromInt64 : x : Int64 ->  Expression


#####CompiledName: FromInt64


####Описание
Конвертирует число типа Int64 в Expression. По сути является оберткой над Expression.FromInt64

----------

####Пример

    Expression.FromInt64 3L
    |> Infix.format
    |> printfn "%s"

####Вывод

	3

