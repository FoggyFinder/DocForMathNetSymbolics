#Operators.fromIntegerFraction

	val fromIntegerFraction : n : BigInteger -> d : BigInteger ->  Expression


#####CompiledName: fromIntegerFraction


####Описание
Конвертирует дробь, представленную двумя числами типа BigInteger в Expression, где:

***n*** - числитель

***m*** - знаменатель

----------

####Пример

    let num = new bigint 100
    let den = new bigint 25 
    Operators.fromIntegerFraction num den
    |> Infix.format
    |> printfn "%s"

####Вывод

	4