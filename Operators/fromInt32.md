#Operators.fromInt32

	val fromInt32 : x : Int32 ->  Expression


#####CompiledName: fromInt32


####Описание
Конвертирует число типа Int32 в Expression

----------

####Пример

    Operators.fromInt32 32
    |> Infix.format
    |> printfn "%s"

####Вывод

	32