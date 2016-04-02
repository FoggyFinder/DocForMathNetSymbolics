#Rational.variables 

	val variables: x : Expression -> HashSet<Expression>


#####CompiledName: Variables


####Описание
Получает список выражений для заданного рационального выражения

----------

####Пример
    
    "(3/x^2 + 5*x)*(2*x+7)/(3*y-5)"
    |> Infix.parseOrUndefined
    |> Rational.variables
    |> Seq.map(Infix.format)
    |> Seq.iter(printfn "%s")
    
####Вывод
    
    7 + 2*x
    3/x^2 + 5*x
    y
    

