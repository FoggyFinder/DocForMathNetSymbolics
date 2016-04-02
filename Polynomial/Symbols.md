#Polynomial.symbols

	val symbols : xs : Expression list -> HashSet<Expression>


#####CompiledName: Symbols


####Описание

Преобразует список выражений в множество (System.Collections.Generic.HashSet)

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let x = symbol "x"
    let a = symbol "a"
    
    Polynomial.symbols [x;a;x]
    |> Seq.iter(print)
    

####Вывод
    
    x
    a








