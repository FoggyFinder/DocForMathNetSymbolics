#Structure.map

	val map: f : (Expression -> Expression) -> _arg1 : Expression ->  Expression


#####CompiledName: Map


####Описание

Применяет заданную функцию к каждому операнду дерева выражений и возвращает новое выражение.


----------

####Пример

    
    let str = "3*sin(2*x) + y^3"
    let expr = str |> Infix.parseOrUndefined
    
    let print exp = 
    	exp |> Infix.format |> printfn "%s"
    
    expr 
    |> print
    
    let nexpr = Structure.map (fun x -> x * 4Q) expr
    nexpr
    |> print
    

####Вывод

    y^3 + 3*sin(2*x)
    4*y^3 + 12*sin(2*x)

