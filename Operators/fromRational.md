#Operators.fromRational

	val fromRational : x : BigRational ->  Expression


#####CompiledName: fromRational


####Описание
Конвертирует число типа BigRational (MathNet.Numerics) в Expression

----------

####Пример

    let rat = BigRational.Zero
    Operators.fromRational rat
    |> Infix.format
    |> printfn "%s"

####Вывод

	0