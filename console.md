# console

노드의 console에는 여러가지 메서드가 있다. 

## log

기본형 

~~~javascript
console.log('문자 출력')
~~~

템플릿을 이용해 다음과 같이 표현할 수 있다.

~~~~javascript
console.log('숫자 : %d + %d = %d', 10, 25, 10 + 29);
console.log('문자열 : %s', Hello world');
~~~~

## time, timeEnd

어떤 로직의 시작시간과  종료시간을 출력한다.  이때 () 안에 들어가는 라벨은 같은아야 한다.

~~~javascript
console.time('반복문');
for (let i = 0; i < 10; i++) {
    i++;
}
console.timeEnd('반복문');
~~~

~~~bash
반복문: 0.190ms
~~~

## trace

에러를 추적한다. 

~~~javascript
console.trace('에러 추적');
}
function a() {
    b();
}
a();
~~~



~~~~bash
Trace: 에러 추적
    at b (/Users/jskim86/Documents/javascript/node_ex/console.js:19:13)
    at a (/Users/jskim86/Documents/javascript/node_ex/console.js:22:5)
    at Object.<anonymous> (/Users/jskim86/Documents/javascript/node_ex/console.js:24:1)
    at Module._compile (internal/modules/cjs/loader.js:776:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:787:10)
    at Module.load (internal/modules/cjs/loader.js:653:32)
    at tryModuleLoad (internal/modules/cjs/loader.js:593:12)
    at Function.Module._load (internal/modules/cjs/loader.js:585:3)
    at Function.Module.runMain (internal/modules/cjs/loader.js:829:12)
    at startup (internal/bootstrap/node.js:283:19
~~~~

