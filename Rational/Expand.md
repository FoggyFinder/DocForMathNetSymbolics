#Rational.expand

	val expand: x : Expression ->  Expression


#####CompiledName: Expand


####Описание
"Разворачивает" числитель и знаменатель дроби

----------

####Пример
    
    "(3/x^2 + 5*x)*(2*x+7)/(3*x-5)"
    |> Infix.parseOrUndefined
    |> Rational.expand
    |> Infix.format
    |> printfn "%s"
    

####Вывод

    (21 + 6*x + 35*x^3 + 10*x^4)/(-5*x^2 + 3*x^3)
