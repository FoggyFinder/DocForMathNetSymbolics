#Calculus.tangentLine

	val tangentLine : symbol : Expression -> value : Expression -> expression : Expression ->  Expression


#####CompiledName: TangentLine


####Описание
	
Находит касательную к функции (***expression***) для заданного символа (***symbol***)
в определенной точке (***value***)

----------

####Пример

    let expr = "(x-2)*(x+3)" |> Infix.parseOrUndefined
    let x = symbol "x"
    let value = 4Q
    
    Calculus.tangentLine x value expr
    |> Infix.format
    |> printfn "%s"

####Вывод

    -22 + 9*x






