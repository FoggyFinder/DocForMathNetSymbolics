#Calculus.differentiate

	val differentiate : symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: Differentiate


####Описание
	
Возвращает производную функции по аргументу, заданному в виде символа ***symbol***
. Так как вычисляется не частная производная, то все остальные символы в выражении, условно
приравниваются к константам.

----------

####Пример

    let f = "sin(2*x^2) + 3*x" |> Infix.parseOrUndefined
    let x = symbol "x"
    let f'x = Calculus.differentiate x f
    
    f'x
    |> Infix.format
    |> printfn "%s"

####Вывод

    3 + 4*x*cos(2*x^2)





