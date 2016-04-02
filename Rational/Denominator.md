#Rational.denominator

	val denominator: : _arg1 : Expression ->  Expression


#####CompiledName: Denominator


####Описание
Возвращает знаменатель дроби

----------

####Пример

    "3/x^4"
    |> Infix.parseOrUndefined
    |> Rational.denominator
    |> Infix.format
    |> printfn "%s"

####Вывод

    x^4



