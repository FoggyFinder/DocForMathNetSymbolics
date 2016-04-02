#Numbers.lcm

	val lcm : ax : Expression list ->  Expression


#####CompiledName: LeastCommonMultiple


####Описание

Находит наименьший общий множитель для списка целых чисел заданных в виде выражений
(Expression)

----------

####Пример

    Numbers.lcm [4Q;2Q;3Q;5Q]
    |> Infix.format
    |> printfn "%s"

####Вывод

    60




