#NumericLiteralQ.FromString

	val FromString : str : String ->  Expression


#####CompiledName: FromString


####Описание
Конвертирует строку в Expression. Для преобразования использует BigRational.Parse.
Таким образом, можно использовать только строковые представления целых чисел.

----------

####Пример

    NumericLiteralQ.FromString "9876543210"
    |> Infix.format
    |> printfn "%s"

####Вывод

	9876543210

