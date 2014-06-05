
# appium-js

* appium은 android나 ios 앱의 UI테스트를 쉽게 작성할 수 있도록 도와주는 테스트 프래임워크이다. 이의 js bind에 대해 간단히 정리한다.

* 장점
	* node인 만큼 compile이 필요없다 
	* blackbox test다.
	* android project와 별개로 독립된 테스트 프로젝트를 구성할 수 있다. 
* 단점 
	* UI테스트인 만큼 깨지기 쉽다.
	* blackbox 테스트이지만 element를 찾기 위한 android project의 내부 구조에 대한 이해가 여전히 필요하다.
	* async라 코드가 드럽다 -_- 


## install

* android 개발환경 setup
	* sdk
	* adt or android studio
* appium 설치
	* node install -g appium 
	* **or** download & install
* genymotion  (emulator보다 빠른 runtime 환경)
	* 가입 -> 다운로드 -> install 	

## setup

```
$> appium
```


## 테스트 실행

```
$> node tc***.js
```

## 추가 질문

[Not Answered]

* coffeescript로 tc작성은 어떻게 할까?
* 

## reference

* monacle
* yiewd

