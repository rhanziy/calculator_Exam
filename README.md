# calculator_Exam 

> onyl css만 이용한 계산기 예제. 유튜브보고 신기해서 따라해봤다.



------------
user-select: none; 더블클릭이나 드래그에 반응 X

<span class="num equal" onclick="document.calc.txt.value = eval(calc.txt.value)"><i>=</i></span>
eval함수는 사용을 지양하는걸 권고한다. 
eval 함수는 expression 인자에 string 값을 넣으면 해당 값을 그대로 실행하여 결과를 출력해 준다.
> string 타입인데도 불구하고, eval 로 실행하면 그대로 연산 값을 얻을 수 있다는 편리함이 있다. 단순 연산뿐 아니라 내장함수, 객체도 실행가능하다.

출처: MDN
eval()은 인자로 받은 코드를 caller의 권한으로 수행하는 위험한 함수입니다. 
악의적인 영향을 받았을 수 있는 문자열을 eval()로 실행한다면, 당신의 웹페이지나 확장 프로그램의 권한으로 사용자의 기기에서 악의적인 코드를 수행하는 결과를 초래할 수 있습니다. 
또한, 제3자 코드가 eval()이 호출된 위치의 스코프를 볼 수 있으며, 이를 이용해 비슷한 함수인 Function으로는 실현할 수 없는 공격이 가능합니다.
