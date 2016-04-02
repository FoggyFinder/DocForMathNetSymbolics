#Operators.real

	val real : floatingPoint : Double ->  Expression


#####CompiledName: real


####Описание

Конвертирует значение типа float (double) в выражение.
    
----------

####Пример
    
    Operators.real 10.7
    |> Infix.format
    |> printfn "%s"

####Вывод

    10,7




