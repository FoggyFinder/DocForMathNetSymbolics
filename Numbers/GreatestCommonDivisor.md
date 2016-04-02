#Numbers.gcd

	val gcd : ax : Expression list ->  Expression


#####CompiledName: GreatestCommonDivisor


####Описание

Находит наибольший общий делитель для списка целых чисел заданных в виде выражений
(Expression)

----------

####Пример

    Numbers.gcd [36Q;60Q;180Q]
    |> Infix.format
    |> printfn "%s"

####Вывод

    12




