#Polynomial.coefficient

	val coefficient: symbol : Expression -> k : Int32 -> x : Expression ->  Expression


#####CompiledName: Coefficient


####Описание
Возвращает ***k*** - ый коэффициент полинома для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "3 + 4*x + 6*x*y + 12*x^2" |> Infix.parseOrUndefined
    let x = symbol "x"
    let k = 1
    
    Polynomial.coefficient x k expr
    |> Infix.format
    |> printfn "%s"

####Вывод
    
    4 + 6*y
