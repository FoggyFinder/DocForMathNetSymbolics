#Operators.fromInt64

	val fromInt64 : x : Int64 ->  Expression


#####CompiledName: fromInt64


####Описание
Конвертирует число типа Int64 в Expression

----------

####Пример

    Operators.fromInt64 64L
    |> Infix.format
    |> printfn "%s"

####Вывод

	64

