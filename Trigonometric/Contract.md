#Trigonometric.contract

	val contract : x : Expression ->  Expression


#####CompiledName: Contract


####Описание
	
"Сокращает" тригонометрическое выражение

----------

####Пример

    "sin(x)^2*cos(x)^2 - 1/8 + sin(x) + sin(y)"
    |> Infix.parseOrUndefined
    |> Trigonometric.contract
    |> Infix.format
    |> printfn "%s"
    

####Вывод

    sin(x) + sin(y) - (1/8)*cos(4*x)





