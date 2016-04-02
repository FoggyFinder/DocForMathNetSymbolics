#Rational.simplify

	val simplify: symbol : Expression -> x : Expression ->  Expression


#####CompiledName: Simplify


####Описание
Упрощает дробь относительно заданного символа

----------

####Пример
    
    let expr = "(x+2)/(x+1) + (x-1)/(x-2)" |> Infix.parseOrUndefined
    let sim = expr |> Rational.simplify (symbol "x")
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    sim
    |> Infix.format
    |> printfn "%s"

####Вывод
    
    (-1 + x)/(-2 + x) + (2 + x)/(1 + x)
    (-5 + 2*x^2)/(-2 - x + x^2)


