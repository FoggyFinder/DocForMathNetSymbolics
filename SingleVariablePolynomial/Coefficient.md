#SingleVariablePolynomial.coefficientSV

	val coefficientSV: : symbol : Expression -> k : Int32 -> x : Expression ->  Expression


#####CompiledName: Coefficient


####Описание
Возвращает ***k*** - ый коэффициент для заданного символа (***symbol***)

----------

####Пример
    
    let expr = "3 + 4*x + 12*x^2" |> Infix.parseOrUndefined
    let x = symbol "x"
    let k = 2
    
    SingleVariablePolynomial.coefficientSV x k expr
    |> Infix.format
    |> printfn "%s"

####Вывод
    
    12
    