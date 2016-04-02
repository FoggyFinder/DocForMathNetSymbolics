#Infix.formatStrictWriter

	val formatStrictWriter : writer : TextWriter -> expression : Expression ->  unit


#####CompiledName: FormatStrictWriter


####Описание:
	
Записывает дерево выражений (Expression) в точном соответствии в указанный TextWriter (System.IO).

----------

####Пример
    
    let str = "tan(x)+sin(y)/2+z^4"
    let expr = str |> Infix.parseOrUndefined 
    
    let sw = new StreamWriter("formatStrict.txt")
    Infix.formatStrictWriter sw expr 
    sw.Close()

#####Вывод

В файле formatStrict.txt записано:

    z^4 + (1/2)*sin(y) + tan(x)