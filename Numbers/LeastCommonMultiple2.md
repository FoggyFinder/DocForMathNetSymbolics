#Numbers.lcm2

	val lcm2 : u : Expression -> v : Expression ->  Expression


#####CompiledName: LeastCommonMultiple2


####Описание

Определяет наименьший общий множитель для двух целых чисел.


----------

####Пример

    Numbers.lcm2 3Q 4Q
    |> Infix.format
    |> printfn "%s"

####Вывод

    12





