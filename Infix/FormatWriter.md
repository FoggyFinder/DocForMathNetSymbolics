#Infix.formatWriter

	val formatWriter : writer : TextWriter -> expression : Expression ->  unit


#####CompiledName: FormatWriter


####Описание
	
Записывает дерево выражений (Expression) в указанный TextWriter (System.IO) в читабельном виде .

----------

####Пример

    let str = "tan(x)+sin(y)/2+z^4"
    let expr = str |> Infix.parseOrUndefined 
    
    let sw = new StreamWriter("format.txt")
    Infix.formatStrictWriter sw expr 
    sw.Close()

####Вывод
В файле format.txt записано:

    z^4 + (1/2)*sin(y) + tan(x)



