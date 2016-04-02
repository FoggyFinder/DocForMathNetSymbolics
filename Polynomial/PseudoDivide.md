#Polynomial.pseudoDivide

	val pseudoDivide : symbol : Expression -> u : Expression -> v : Expression ->  Expression * Expression * Expression


#####CompiledName: PseudoDivide


####Описание

Псевдо-деление полиномов (не требует коэффициент делимости).
Возвращает кортеж из трех элементов - псевдо-частное q,
псевдо-остаток r, множитель b, такие, что:

     b*u = q*v+r

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let u = "3*x^3 + x^2 + x + 5" |> Infix.parseOrUndefined
    let v = "5*x^2 - 3*x + 1" |> Infix.parseOrUndefined
    let x = symbol "x"
    
    printf "u: "
    print u
    
    printf "v: "
    print v
    
    Polynomial.pseudoDivide x u v 
    |> Microsoft.FSharp.Reflection.FSharpValue.GetTupleFields
    |> Seq.map(fun x -> x:?> Expression)
    |> Seq.iter(print)
    
####Вывод
    
    u: 5 + x + x^2 + 3*x^3
    v: 1 - 3*x + 5*x^2
    14 + 15*x
    111 + 52*x
    25
    
    





