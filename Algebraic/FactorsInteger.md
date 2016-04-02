#Algebraic.factorsInteger

	val factorsInteger : _arg1 : Expression ->  BigInteger * Expression list


#####CompiledName: FactorsInteger


####Описание
	
Отделяет целый множитель из выражения, который и возвращает как первый элемент кортежа.
Второй - список оставшихся множителей. 

----------

####Пример

    let expr = "1/5*sin(x)*(x+2)*cos(3*t)" |> Infix.parseOrUndefined
    
    let fInt, xs = Algebraic.factorsInteger expr
    
    printfn "%A" fInt
    xs
    |> List.map(Infix.format)
    |> List.iter(printfn "%s")

####Вывод

    1
    1/5
    2 + x
    sin(x)
    cos(3*t)





