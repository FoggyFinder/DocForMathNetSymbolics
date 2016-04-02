#Infix.format

	val format : expression : Expression ->  String


#####CompiledName: Format


####Описание
	
Преобразует математическое выражение в форматированную строку, для читабельного вывода

----------

####Пример

    let str = "4*x*x + 2*sin(3*y) + 5*cos(x)"
    let expr = str |> Infix.parseOrUndefined
    expr |> Infix.format |> printfn "%s"

####Вывод

    4*x^2 + 2*sin(3*y) + 5*cos(x)



