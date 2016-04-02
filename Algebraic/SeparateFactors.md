#Algebraic.separateFactors

	val separateFactors : symbol : Expression -> x : Expression -> Expression * Expression


#####CompiledName: SeparateFactors


####Описание
	
Группирует множители выражения на две части - в одной находятся те,
которые содержат в себе символ ***symbol***, во второй - те, в которых он не встречается.
Части возвращаются в виде кортежа.

----------

####Пример

    let x = symbol "x"
    
    let expr = "4*(x+2)*cos(3*t)*sin(z+x)" |> Infix.parseOrUndefined
    
    let f,s = Algebraic.separateFactors x expr
    
    [f;s]
    |> List.map(Infix.format)
    |> List.iter(printfn "%s")

####Вывод

    4*cos(3*t)
    (2 + x)*sin(x + z)


