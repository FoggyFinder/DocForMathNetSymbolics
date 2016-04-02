#SingleVariablePolynomial.degreeMonomialSV

	val degreeMonomialSV: symbol : Expression -> _arg1 : Expression ->  Expression


#####CompiledName: MonomialDegree


####Описание
Определяет степень монома с заданной переменной (***symbol***)

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let expr = "4*y^3" |> Infix.parseOrUndefined
    let y = symbol "y"
    
    print expr
    
    SingleVariablePolynomial.degreeMonomialSV y expr
    |> Infix.format
    |> printfn "%s" 
    
####Вывод
    
    4*y^3
    3
    





