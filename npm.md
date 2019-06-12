# nvm이란

nvm이란 nodeJs의 버전을 관리하는 툴인다.  원하는 버전의 nodeJs를 설치  및 제거 할 수 있으며 버전을 업그레이드 할 수 있다.

github 에서 관련 프로세스를 설치한다.

<https://github.com/nvm-sh/nvm> 

설치 안내대로 설치를 진행한다. 

# nvm 제거

nvm 을 제거하기전에 먼저 nodeJs를 제거한 후 숨겨져 있는 nvm 디렉터리를 제거해 준다. 

~~~
# rm -rf $NVM_DIR  →  $NVM_DIR은 nvm 폴더 경로 환경변수이다.
~~~

# node.js 제거하기

~~~
// nvm uninstall <node version>
# nvm uninstall 10.14.2  → 10.14.2를 제거한다.
~~~

만약 활성화된 node가 있다고 나온다면  아래 명령어를 입력한다. 

~~~ 
# nvm deactive  
# nvm uninstall 10.14.2  → 정상적으로 제거된다.
~~~





