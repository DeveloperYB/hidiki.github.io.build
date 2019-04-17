# * 리엑트 장단점 및 사용하기 좋은 예시

## **리엑트 장점**

### 1. 리엑트는 라이브러리다.
> 리엑트는 주된 비교대상인 뷰, 앵귤러 (프레임워크) 와 다르게 라이브러리 이므로,
크게 아키텍쳐링을 하는데 있어서 제약이나 자유도가 적지 않다. 이점은 단점으로도 작용할 수 있지만 아키텍쳐링 유연성을 좋아하는 개발자에게는 재미를 느끼는 큰 요소로 생각된다.

### 2. 리엑트는 pure javascript에 가깝다.
> 자바스크립트를 그대로 사용하는 점에 있어서, 크게 더 배울 요소가 없다. 러닝커브가 낮다고 생각한다. (물론 부가적으로 따라오는 Redux, React-router, Saga, Thunk 등 써드파티 라이브러리는 어렵게 느껴질 수 있다.)

### 3. 리엑트는 정말 작은 단위로 컴포넌트를 쪼갤수 있다.
> 리엑트는 작은 단위로 컴포넌트를 나뉘어서 개발을 할 수 있다. 마치 레고블럭을 조립하듯이 여러 컴포넌트 블럭을 합쳐서 프로젝트를 형성한다. 이점에서 코드 재사용성이 정말 좋다고 생각한다.

### 4. 리엑트는 인기가 많다.
> Facebook, Dropbox, Khan Academy, CodeAcademy, Netflix, Airbnb, PayPal, Walmart, Tesla Motors 등 굵직굵직한 업체에서 채택을 할 만큼,
프론트 엔드 개발을 위한 매우 우수한 도구라는 것이 입증되었다고 본다. 또한, 많은 개발자들이 사용을 하고 있기 때문에 새로운 example 코드가 계속 생겨나고 발전의 가능성이 높다고 본다.

### 5. Virtual Dom - 가상 돔 트리
> 웹 브라우저에서 돔 트리를 해석하고 다시 새로운 화면을 그려준다는 것(렌더링) 은 생각보다 많은 과정이 필요하다.\
(렌더트리를 재생성 - 각 모든 요소들 스타일 다시 계산 - 레이아웃 재생성 - 페인팅, 렌더링)\
위 과정 처럼 브라우저는 많은 연산을 해야되지만 리엑트에서 지원하는 가상 돔은 변화된 부분을 먼저 체크해서 변화된 부분의 결과만 Dom에 전달 하기때문에 위 과정을 연산하는 것보다 효율적이다.\
(참고로, 그렇다고 리엑트가 빠르다는 아닙니다. 필자가 만들었던 DCE(컨탠츠 에디터툴)라는 프로젝트의 경우 코드를 잘못구현하여서 엄청 버벅거리는 이슈도 있었습니다.)

### 6. SEO
> 서버사이드 렌더링에 리엑트는 최적화 되어있다. 애초에 리엑트는 서버사이드 렌더링을 고려해서 설계가 되어있다. "ReactDOMServer.renderToString" 라는 함수로 서버 사이드에서 사용하는 렌더링 함수를 지원한다.

### 7. React Native 로 쉬운 전환
> 리엑트 네이티브는 리엑트를 기반으로한 모바일 개발 프레임워크인데, 리엑트 웹앱에 사용되던, 대부분의 비즈니스 로직을 리엑트 네이티브 모바일 앱에서 재사용할 수 있다.

---

## **리엑트 단점**

필자가 생각하는 리엑트의 가장 큰 단점은 아무래도 정확한 모범사례라고 지칭할 수 있는 코드가 없다는 점이라고 본다. 다른 비교 프레임워크에 비해서 아키텍쳐링에 유연하고, 어떤 써드파티 라이브러리를 사용하냐에 따라서도 프로젝트 구현이 제각각 달라지기 때문에 어떤 방법이 옳다, 어떤 방법이 모범이다 라고 딱 꼽을수가 없다.\
앞서 말했듯이, 장점이자 가장 큰 단점이라고 본다.

---

## **리엑트 사용하기 좋은 예시**

리엑트 공식 문서에는 시간이 지남에 따라 변하는 데이터로 만들어진 대규모 프로그램을 제작하기 위해 고안되었다고 한다.

따라서 리엑트를 사용하면 좋은 예시를 들자면,

- 대규모 프로그램
- SPA
- 동적으로 계속 변화하는 웹 (데이터 시각화)
- 복잡한 UI

위 4개라고 생각한다.

---