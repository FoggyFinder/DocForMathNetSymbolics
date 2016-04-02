#Structure.freeOfSet

	val freeOfSet: symbols : HashSet<Expression> -> x : Expression ->  Boolean


#####CompiledName: IsFreeOfSet


####Описание

Проверяет, входит ли множество заданных символов (***symbols***) в выражение

----------

####Пример
    
    let hs = HashSet([symbol "y"; symbol "z"])
    let xs = ["2*x*y";"(3-x)/(4+x)";"3+z/x+2"]
    
    xs
    |> List.map(Infix.parseOrUndefined)
    |> List.map(fun v -> Infix.format v, Structure.freeOfSet hs v)
    |> List.iter(fun (v,r) -> printfn "%s - %b" v r) 
    
####Вывод
    
    2*x*y - false
    (3 - x)/(4 + x) - true
    5 + z/x - false
    
    
    
