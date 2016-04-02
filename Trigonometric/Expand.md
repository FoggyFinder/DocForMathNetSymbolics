#Trigonometric.expand

	val expand : x : Expression ->  Expression


#####CompiledName: Expand


####Описание
	
"Разворачивает" тригонометрическое выражение на слагаемые

----------

####Пример

    "sin(2*x)+cos(2*x)"
    |> Infix.parseOrUndefined
    |> Trigonometric.expand
    |> Infix.format
    |> printfn "%s"


####Вывод

    -sin(x)^2 + 2*sin(x)*cos(x) + cos(x)^2



