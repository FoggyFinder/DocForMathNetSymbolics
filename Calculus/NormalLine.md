#Calculus.normalLine

	val normalLine : symbol : Expression -> value : Expression -> expression : Expression ->  Expression


#####CompiledName: NormalLine


####Описание
	
Определяет нормаль к функции ***expression***, заданную выражением Expression с указанием
аргумента функции (***symbol***) в заданной точке (***value***).

Нормалью к кривой называется прямая, проходящая через точку касания перпендикулярно касательной


----------

####Пример

    let expr = "(x-2)*(x+3)" |> Infix.parseOrUndefined
    let x = symbol "x"
    let value = 4Q
    
    Calculus.normalLine x value expr
    |> Infix.format
    |> printfn "%s"

####Вывод

    130/9 - (1/9)*x






