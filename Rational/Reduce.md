#Rational.reduce

	val reduce: x : Expression ->  Expression


#####CompiledName: Reduce


####Описание

Пытается удалить общие множители из всех членов рационального выражения

----------

####Пример
    
    "(8*a*x + 6*a*x^2)/(4*x*a)"
    |> Infix.parseOrUndefined
    |> Rational.reduce 
    |> Infix.format
    |> printfn "%s"
    
####Вывод
    
    (1/2)*(4 + 3*x)
    