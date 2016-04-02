#Trigonometric.substitute

	val substitute : x : Expression ->  Expression


#####CompiledName: Substitute


####Описание
	
Заменяет тангенс, котангенс, секанс, косеканс на синус и косинус

----------

####Пример

    "tan(x)"
    |> Infix.parseOrUndefined
    |> Trigonometric.substitute
    |> Infix.format
    |> printfn "%s"
    

####Вывод
    
    sin(x)/cos(x)