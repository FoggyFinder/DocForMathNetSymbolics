#NumericLiteralQ.FromInt32

	val FromInt32 : x : Int32 ->  Expression


#####CompiledName: FromInt32


####Описание
Конвертирует число типа Int32 в Expression. По сути является оберткой над Expression.FromInt32

----------

####Пример

    Expression.FromInt32 2
    |> Infix.format
    |> printfn "%s"

####Вывод

	2



