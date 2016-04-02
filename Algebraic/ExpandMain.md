#Algebraic.expandMain

	val expandMain : _arg1 : Expression ->  Expression


#####CompiledName: ExpandMain


####Описание
	
"Разворачивает" математическое выражение на слагаемые только относительно главного оператора.

----------

####Пример
    
    let expr = "3*(x+y)*(x+1)*(y+3)" |> Infix.parseOrUndefined
    
    Algebraic.expandMain expr
    |> Infix.format
    |> printfn "%s"

####Вывод


    9*x + 9*x^2 + 9*y + 12*x*y + 3*x^2*y + 3*y^2 + 3*x*y^2


----------

####Дополнительная информация

----------

Так как по описанию отличие от функции [Algebraic.expand](Expand.html) может быть
не совсем понятно, будет уместно привести следующий пример:

    let expr = "3*((x+y)*(x+1)+(y+3)*(x-2))" |> Infix.parseOrUndefined
    
    Algebraic.expandMain expr
    |> Infix.format
    |> printfn "%s"
    
    Algebraic.expand expr
    |> Infix.format
    |> printfn "%s"

Вывод:

    3*(-2 + x)*(3 + y) + 3*(1 + x)*(x + y)
    -18 + 12*x + 3*x^2 - 3*y + 6*x*y

