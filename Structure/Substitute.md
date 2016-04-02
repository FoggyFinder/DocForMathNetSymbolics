#Structure.substitute

	val substitute: y : Expression -> r : Expression -> x : Expression ->  Expression


#####CompiledName: Substitute


####Описание

Заменяет одну часть в выражении (Expression) на другую 

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "3*x*y + 2*x + sin(x)*3*x*y" |> Infix.parseOrUndefined
    let _from = "3*x*y" |> Infix.parseOrUndefined
    let _to = "2*z" |> Infix.parseOrUndefined
    
    print expr 
    printf "Replace:\nOld value: "
    print _from
    printf "New value: "
    print _to
    
    Structure.substitute _from _to expr
    |> print
    
    
####Вывод
    
    2*x + 3*x*y + 3*x*y*sin(x)
    Replace:
    Old value: 3*x*y
    New value: 2*z
    2*x + 2*z + 3*x*y*sin(x)
    