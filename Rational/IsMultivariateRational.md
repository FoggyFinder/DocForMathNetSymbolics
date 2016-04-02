#Rational.isRationalMV

	val isRationalMV : symbols : HashSet<Expression> -> x : Expression ->  Boolean


#####CompiledName: IsMultivariateRational


####Описание
	
Проверяет, является ли выражение рациональным для заданного множества символов.

----------

####Пример
    
    let hs = HashSet([symbol "x"; symbol "y"])
    
    "(2*x+7)/(3*y-5)"
    |> Infix.parseOrUndefined
    |> Rational.isRationalMV hs
    |> printfn "%b"
    
####Вывод
    
    true
    
    


