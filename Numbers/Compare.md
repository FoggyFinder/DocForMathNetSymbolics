#Numbers.compare

	val compare : x : Expression -> y : Expression -> Int32


#####CompiledName: Compare


####Описание

Сравнивает два выражения, возвращает:

    x > y -> 1
    x = y -> 0 
    x < y -> -1

Операция сравнения реализована только для чисел и +/- infinity (бесконечности).

----------

####Пример

    let data = [1Q; 2Q; 3Q]
    let rev = data |> List.rev
    
    let printXY x y = 
    printfn "%A compare %A = %i"
     (Infix.format x) (Infix.format y) (Numbers.compare x y)
    
    List.iter2(printXY) data rev

####Вывод

    "1" compare "3" = -1
    "2" compare "2" = 0
    "3" compare "1" = 1




