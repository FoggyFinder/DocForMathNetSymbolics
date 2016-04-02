#Rational.numerator

	val numerator: _arg1 : Expression ->  Expression


#####CompiledName: Numerator


####Описание
Возвращает числитель дроби

----------

####Пример

    "3/x^4"
    |> Infix.parseOrUndefined
    |> Rational.numerator
    |> Infix.format
    |> printfn "%s"

####Вывод

    3



