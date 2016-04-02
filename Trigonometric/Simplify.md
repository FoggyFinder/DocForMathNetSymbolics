#Trigonometric.simplify

	val simplify : x : Expression ->  Expression 


#####CompiledName: Simplify


####Описание
	
Упрощает тригонометрическое выражение

----------

####Пример

    "2*sin(x)*cos(x)+sin(2*x)"
    |> Infix.parseOrUndefined
    |> Trigonometric.simplify
    |> Infix.format
    |> printfn "%s"


####Вывод

    2*sin(2*x)




