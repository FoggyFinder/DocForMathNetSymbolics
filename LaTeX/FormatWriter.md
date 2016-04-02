#LaTeX.formatWriter

	val formatWriter : writer : TextWriter -> expression : Expression ->  unit


#####CompiledName: FormatWriter


####Описание
Записывает дерево выражений (Expression) в формате LaTeX в указанный TextWriter (System.IO).

----------

####Пример

    let example = "pi*3*tan(x*y)/4*sin(z)+sin^(2*x)"
    let expr = example |> Infix.parseOrUndefined
    
    let sw = new StreamWriter("LaTeX.txt")
    LaTeX.formatWriter sw expr 
    sw.Close()

####Вывод

В файле LaTeX.txt записано:

    sin^\left(2x\right) + \frac{3}{4}\pi\sin{z}\tan{\left(xy\right)}
