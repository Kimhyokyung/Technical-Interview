# 답
js 에서는 html 태그를 작성하는 문법을 지원하지 않습니다.

그렇기 때문에 jsx 문법을 사용하게 된다면 오류가 나게 됩니다.

어떻게 해야 jsx 문법을 사용하고도 오류가 나지 않게 되느냐를 알고 있으신가요?

바벨은 js 컴파일러 입니다.

이전버전의 문법으로 변경을 해주거나 아직 채택되지않은 신버전의 문법을 사용 가능하게 해주죠.

과연 이게 jsx 와의 무슨 상관이느냐? 라고 궁금하실탠데 그 이유를 알려드리죠

```jsx
return(<div></div>)
```
는
```js
return React.createElement~~~~
```
로 변경됩니다.

그러면 감이 오시나요?

return 되는 태그를 왜 1 개만 작성해야 되는지를 알 수 있습니다.
# 출제 의도
1. 바벨을 알고있는가?
2. 왜 바벨을 사용해야 하는가?
