#Rational.rationalize

	val rationalize: _arg1 : Expression ->  Expression


#####CompiledName: Rationalize


####Описание
Приводит дробь к общему знаменателю.

----------

####Пример
    
    let expr = "x/(2*(x+2)) + (x+1)*(x-2)" |> Infix.parseOrUndefined
    let rat = expr |> Rational.rationalize
    
    expr
    |> Infix.format
    |> printfn "%s"
    
    rat
    |> Infix.format
    |> printfn "%s"

####Вывод
    
    (-2 + x)*(1 + x) + ((1/2)*x)/(2 + x)
    ((1/2)*(x + 2*(-2 + x)*(1 + x)*(2 + x)))/(2 + x)


----------

####Дополнительная информация

Название может ввести в заблуждение, что после применение
функции, [Rational.isRational](IsRational.html) вернет **true**.
На самом деле это не так. Чтобы привести дробь к рациональному виду, нужно
применить [Rational.expand](Expand.html).
