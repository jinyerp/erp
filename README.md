# jinyERP
`jinyERP`는 라라벨 기반으로 생성된 ERP 프로젝트트 입니다. 

## 설치
jinyERP는 2가지 방식으로 프로젝트를 설치 가능합니다.

### 컴포저를 이용한 프로젝트 실행
패키지로 포장된 jinyerp를 컴포저를 통하여 설치 가능합니다. 다음과 같이 명령을 입력합니다.
```
composer create-project --prefer-dist jinyphp/erp 프로젝트명 버젼
```

### 소스로 설치
깃 저장소를 `clone`하여 설치 jinytms 설치가 가능합니다.
```
git clone https://github.com/jinyerp/erp.git
```

clone을 통하여 설치한 경우 몇개의 추가 설정이 필요로 합니다.

##### 환경설정 파일 생성하기
라라벨의 기본 환경설정 파일을 생성합니다. 예제파일을 `.env`로 복사한후에, 설정을 추가합니다.
```
cp .env.sample .env
```

##### 키 생성
```
php artisan key:gen
```

##### 의존성 패키지 설치
소스코드에는 의존되어 있는 패키지들이 설치되어 있지 않습니다. 컴포저를 통하여 의존 패키지를 설치합니다.

```
composer install
```

의존 패키지를 설치하게 되면 루트에 `vendor` 폴더가 생성되는 것을 확인할 수 있습니다.






