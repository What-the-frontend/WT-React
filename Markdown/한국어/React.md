React란
===

원래의 DOM(Document Object Model)은 변경사항이 생길 때마다 페이지 전체를 새로 랜딩한다. 따라서 자원낭비가 심하고 DOM자체는 속도가 빠르지만  속도가 느려지는 경우가 있다. 이 때 React를 사용하면 Virtual DOM을 사용해서 바뀐 부분만 랜딩을 새로하는 것이 가능하다. 따라서 성능 상에서 큰 이점을 가져올 수 있기 때문에 React를 사용한다. React는 node를 기반으로 동작하고 npm을 이용해서 프로젝트를 설정할 수 있다.

## Props

변하지 않는 값을 데이터를 다룰 때 사용한다. parent 컴포넌트에서 child 컴포넌트로 데이터를 전달할 때 사용한다.

## State

컴포넌트에서 유동적인 데이터를 관리할 때 사용한다. 예를 들어서 진행도에 따라서 변화하는 상태바가 있다고 한다면, 상태바는 유동적으로 계속 변화해야한다. 이럴 때 state를 사용한다.
state값은 class내에서 constructor를 선언하고 this.state를 이용해서 key : value을 지정해준다. 그 후에 다른 곳에서 state값에 유동적으로 접근할 때는 함수를 하나 생성한다. 그 후에 constructor내에서 그 함수를 bind해주고 setState함수를 이용해서 값을 조절할 수 있다.

## Iterator(반복문)

중복되는 컴포넌트가 있는 경우에는 반복문을 통해서 처리할 수 있다.
render()스코프 내에서 return()해주기 전에 배열에 for문을 이용해서 컴포넌트들을 저장하는 방법과 Array의 함수중 하나인 map을 사용한다. (Array.md 참고)