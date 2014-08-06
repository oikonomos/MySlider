**
 * 버전 : 1.2.0
 * 만든 이 : 석상범
 * 만든 일자 : 2014. 8. 5
 * 상하 또는 좌우 화살표 네비게이션 버튼을 추가함.
 * params : opts(JSON)
 * slideHolder: Slide Holder ID
 * Slide : Slide Classname
 * buttonHolder: Button Holder ID
 * speed
 * slidingPlane: horizontal or vertical),
 * period: Timer Duration
 * direction: left or right or up or down
 * isNaviArrow 
 * 이전 버전

**

1. 개발 스토리

* 버전 1.0.0 : 슬라이드와 내비게이션 버튼를 가르키는 포인터 객체를 생성하여 이미지 슬라이드를 구현한다.
* 버전 1.1.0 : 수평면 슬라이딩과 수직면 슬라이딩을 합침.
* 버전 1.1.1 : 슬라이딩 입력 변수들을 JSON으로 바꿈.
* 버전 1.2.0 : 좌우 또는 상하 화살표 네비게이션 버튼을 추가함.


2. 사용법

(1) 슬라이딩에 필요한 초기값을 JSON으로 입력한다.

- Optios Parameters
- params : opts(JSON)
- slideHolder: Slide Holder ID
- Slide : Slide Classname
- buttonHolder: Button Holder ID
- speed
- slidingPlane: horizontal or vertical),
- period: Timer Duration
- direction: left or right or up or down
- isNaviArrow : false or true

(2) 좌우 또는 상하 화살표 내비게이션을 활성활 경우, 왼쪽 또는 위쪽 방향 화살표 이미지의 컨테이너 엘리멘트 id가 first-arrow이고, 오른쪽 또는 아래쪽 화살표 이미지의 컨테이너 엘리멘트 id는 second-arrow이어야만 한다. 만약 이 값이 틀리면 슬라이딩은 오류가 난다.

(3) my-slider-버전.css 스타일 시트와 my-slider-버전.min.js 스크립트를 생성한 다음, MySlider 객체를 생성하면 슬라이딩이 정상적으로 동작한다.

	(예) var ms = new MySlider({
		slideHolder: "slider-holder",
		slide: "slide",
		buttonHolder: "btn-nav-holder",
		speed: 1E3,
		slidingPlane: "horizontal",
		period:2E3,
		direction:"left",
		isNaviArrow: true
	});

