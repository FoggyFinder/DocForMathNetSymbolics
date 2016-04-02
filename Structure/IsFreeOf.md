#Structure.freeOf

	val freeOf: symbol : Expression -> x : Expression ->  Boolean


#####CompiledName: IsFreeOf


####Описание

Проверяет, входит ли заданный символ (***symbol***) в выражение

----------

####Пример
 
    let y = symbol "y"
    let xs = ["2*x*y";"(3-x)/(4+y)";"3+z/x+2"]
    
    xs
    |> List.map(Infix.parseOrUndefined)
    |> List.map(fun v -> Infix.format v, Structure.freeOf y v)
    |> List.iter(fun (v,r) -> printfn "%s - %b" v r)
    
####Вывод
    
    2*x*y - false
    (3 - x)/(4 + y) - false
    5 + z/x - true
    
    
