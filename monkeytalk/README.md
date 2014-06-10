
# Monkeytalk



# Monkey Talk?

* record & play back 스타일의 시나리오 테스트 도구.  
* 안드로이드, ios 동시 지원

## Building Block

* MonkeyTalk는 mobile앱을 위한 Functional Test Platform으로 현재 native & hybrid iOS, 안드로이드 앱을 지원한다. 
크게 MonkeyTalk IDE, MonkeyTalk Agent, MonkeyTalk Script로 3개의 부분으로 구성된다. 
	* IDE - record/play back/creation of script 를 위한 데스크탑 App 
	* Agent - 테스트가 가능하도록 테스트 대상 app에 추가되어야하는 Library
	* Script - 테스트 script 
```
Input username EnterText joe
Input password EnterText "my secret password"
Button LOGIN Tap
```
<MonkeyTalk Script>
```
app.input("username").enterText("joe");
app.input("password").enterText("my secret password");
app.button("LOGIN").tap();
```
<MonkeyTalk Script (js version)>
	* (warning) agent는 production build에는 제외할 것
 
 


## 시작하기

### 설치
* monkeytalk를 다운로드 후 압축을 해제하면 monkeytalk ide, 
	* monkeytalk download
		* https://www.cloudmonkeymobile.com/developer-resources/downloads

* adt 설치
	* aspectj plugin (ajdt) 설치
	* http://download.eclipse.org/tools/ajdt/43/update


### Android 프로젝트 Instrument

* monkeytalk를 사용하기 위해서는 android 프로젝트를 instrument해야한다. 

* configure > ajdt project
* monkeyTalk-agent.jar library를 libs/ 에 복사
* classpath에 추가
	* right-click on monkeyTalk-agent.jar > AspectJ Tools > Add to Aspectpath

* 참고 
	* https://www.cloudmonkeymobile.com/monkeytalk-documentation/monkeytalk-getting-started/install-agent/android

### monkeytalk 프로젝트 설정

* monkeytalk IDE 구동
* monkeytalk 프로젝트 생성
	* sdk path 설정
	* 대상 apk 설정
* connect > device
* install or relaunch > select apk
* Record & PlayBack

## ant에서 monkeytalk 실행하기

### ant에서 monkeytalk용 앱 빌드하기
* https://www.cloudmonkeymobile.com/monkeytalk-documentation/monkeytalk-user-guide/installing-monkeytalk/building-ant

### ant에서 monkeytalk 테스트 하기
* https://www.cloudmonkeymobile.com/monkeytalk-documentation/monkeytalk-user-guide/ant-runner


## CI에서 구동하기(?)

## 테스트 전략(?)





