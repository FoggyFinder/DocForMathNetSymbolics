#Polynomial.partialFraction

	val partialFraction : symbol : Expression -> numerator : Expression -> denominatorFactors : Expression list -> Expression * Expression list


#####CompiledName: PartialFraction


####Описание

Частичное разложение дроби.

----------

####Пример
    
    let print = Infix.format >> printfn "%s"
    
    let x = symbol "x"
    let n = 5*x - 4
    let d = [x-2; x+1]
    
    Polynomial.partialFraction x n d
    |> fun (x,y) -> print x;  y |> Seq.iter(print)
    
####Вывод
    
    0
    2
    3
    
        
    



