# Countdown-Timer
- 2022년 새해까지 남은 기간을 알려주는 타이머이다.  출처: https://github.com/florinpop17/10-projects-10-hours

# 개발 기간 및 환경

+ 기간: 2021.10.20 ~ 2021.10.21

+ OS: Windows 10

+ Tools: VS Code

+ 실행환경: 크롬 웹 브라우저
---------------------------

# 파일 목록
프로그램이 정상적으로 실행되기 위해서는 다음 파일들이 같은 폴더 내에 존재해야 합니다.<br>
그렇지 않을 경우 정상적인 실행을 보장하지 않습니다.<br><br>

> index.html - 실행 파일
> style.css
> script.js
> snow.jpeg - 배경 이미지
<br>


# TestCase
자바스크립트 내부 코드를 살펴보며 학습합니다. (script.js 파일)

1. html 에서 가져온 elements 값 확인.

```javascript
console.log(daysEl);
console.log(hoursEl);
```

결과:
<p class="big-text" id="days">64</p>
<p class="big-text" id="hours">4</p>

> 남은 일수:64 와 시간:4 이 출력됩니다.

2. Date 객체 값 확인.

```javascript
console.log(newYearsDate);
console.log(currentDate);
console.log(newYearsDate-currentDate);
```
<br>

결과:
Sat Jan 01 2022 00:00:00 GMT+0900 (한국 표준시)
script.js:16 Thu Oct 28 2021 20:02:22 GMT+0900 (한국 표준시)
script.js:17 5543857064

> 현재 시각 기준, 2022년 새해 시각이 한국 표준시로 표시됩니다.
> 두 값 차이는 ms(1/1000초) 값 표시됨.

3. setInterval 함수
```javascript
setInterval(countdown, 1000);
```
1초마다 countdowㅜ function 실행 확인.