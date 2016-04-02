#Numbers.min2

	val min2 : u : Expression -> v : Expression ->  Expression


#####CompiledName: Min2


####Описание
Сравнивает два выражения и возвращает минимальный из них.
Операция сравнения реализована только для чисел и +/- infinity (бесконечности).

----------

####Пример

    Numbers.min2 1Q 2Q 
    |> Infix.format
    |> printfn "%s"

####Вывод

	1



