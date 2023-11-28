## 1. 리액트 Hook이 무엇인지 설명해주세요.

- 내가 작성한 코드를 다른 프로그램에 연결해서 그 값이나 기능을 사용하는 것
- 리액트가 제공하는 기능에 연결해서 그 값이나 기능을 사용하는 함수
- 예)
 ```jsx
function MyComponent() {
    const [num, setNum] = useState(0);
    return (
        <button onClick={ () => setNum(num + 1}}>
            {num}
        </button>
    );
}
```
-> 리액트가 관리하는 State에 연결해서 변수처럼 값을 사용
예) useState, useEffect, useRef


## 2. 다음은 리액트 Hook의 규칙에 어긋나는 코드들입니다. 각각의 코드에서 어떤 부분이 잘못되었는지, 어떤 규칙에 위배되는지 설명해주세요.

![image](https://github.com/jisunipark/sprint-part2-team8/assets/148641571/ada53442-4b0f-4074-b9b8-13407ae1ed08)
-> 반드시 리액트 컴포넌트 함수나 커스텀 Hook 함수 안에서 실행되어야 한다.

![image](https://github.com/jisunipark/sprint-part2-team8/assets/148641571/d6c67b2c-1f7e-471c-8587-1a75cefe6667)
-> 반드시 함수의 최상위에서 실행되어야 한다. (반복문이나 조건문에서 쓰면 안 된다.
