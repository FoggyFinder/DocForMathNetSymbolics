#Trigonometric.separateFactors

	val separateFactors : x : Expression ->  Expression 


#####CompiledName: SeparateFactors


####Описание
	
Разделяет произведение на две части. Первая - остаток,
вторая - синусы, косинусы и они в положительной целой степени

----------

####Пример

    "2 * sin(x)^(2/3) *  cos(t)^2 * (sin(x) + 3*cos(y)) "
    |> Infix.parseOrUndefined
    |> Trigonometric.separateFactors
    |> fun (x,y) -> Infix.format x, Infix.format y
    |> fun (x,y) -> printfn "%s\n%s" x y

####Вывод
    
    2*sin(x)^(2/3)*(sin(x) + 3*cos(y))
    cos(t)^2





