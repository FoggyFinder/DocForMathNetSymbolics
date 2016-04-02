#Rational.isRational

	val isRational: symbol : Expression -> x : Expression ->  Boolean


#####CompiledName: IsRational


####Описание
Проверяет, является ли дробь рациональной, относительно
 заданного символа (***symbol***)

----------

####Пример


    "3/x^2 + 5*x"
    |> Infix.parseOrUndefined
    |> Rational.isRational (symbol "x")
    |> printfn "%b"

####Вывод
    
    false




