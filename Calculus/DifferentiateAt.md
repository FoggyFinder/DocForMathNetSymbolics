#Calculus.differentiateAt

	val differentiateAt : symbol : Expression -> value : Expression -> expression : Expression ->  Expression


#####CompiledName: DifferentiateAt


####Описание
	
Вычисляет значение производной по заданному символу (***symbol***)
в заданной точке (***value***)

----------

####Пример

    let f = "3*x^3" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    let point = 2Q
    let f'x = Calculus.differentiateAt x point f
    
    printfn "f (x) = %s" (Infix.format f)
    
    Calculus.differentiate x f
    |> Infix.format
    |> printfn "f'(x) = %s"

    printfn "f'(%s) = %s" 
    	(Infix.format point) (Infix.format f'x)

####Вывод

    f (x) = 3*x^3
    f'(x) = 9*x^2
    f'(2) = 36
