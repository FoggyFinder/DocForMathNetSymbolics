#LaTeX.format

	val format: expression : Expression -> String


#####CompiledName: Format


####Описание
Форматирует дерево выражений (Expression) в строку в формате LaTeX.

----------

####Пример

    let example = "pi*3*tan(x*y)/4*sin(z)+sin^(2*x)"
    let expr = example |> Infix.parseOrUndefined
    expr |> Infix.formatStrict |> printfn "%s"
    expr |> LaTeX.format |> printfn "%s"

####Вывод

    sin^(2*x) + (3/4)*pi*sin(z)*tan(x*y)
    sin^\left(2x\right) + \frac{3}{4}\pi\sin{z}\tan{\left(xy\right)}

