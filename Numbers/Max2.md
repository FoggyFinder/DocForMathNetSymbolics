#Numbers.max2

	val max2 : u : Expression -> v : Expression ->  Expression


#####CompiledName: Max2


####Описание
Сравнивает два выражения и возвращает максимальный из них.
Операция сравнения реализована только для чисел и +/- infinity (бесконечности).

----------

####Пример

    Numbers.max2 2Q 5Q
    |> Infix.format
    |> printfn "%s"

####Вывод

	5



