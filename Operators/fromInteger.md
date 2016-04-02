#Operators.fromInteger

	val fromInteger : x : BigInteger ->  Expression


#####CompiledName: fromInteger


####Описание
Конвертирует число типа BigInteger (System.Numerics) в Expression

----------

####Пример

    let big = new bigint 100 
    Operators.fromInteger big
    |> Infix.format
    |> printfn "%s"

####Вывод

	100