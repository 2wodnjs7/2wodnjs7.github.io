## 1. Github Page 생성

github의 무료 블로그 호스팅 서비스를 이용해 2wodnjs7.github.io 라는 이름의 Remote Repository를 생성하였다.
그 후 내 컴퓨터에 Local Repository를 생성한 후 연동하였다.
```sh
git remote add origin https://github.com/2wodnjs7/2wodnjs7.github.io.git
```


## 2. Jekyll 설치

정적 사이트 생성기인 Jekyll를 이용한다.
먼저 Jekyll를 설치한다.
```sh
gem install jekyll bundler
```
그리고 현재 디렉토리(.)에 Jekyll을 설치한다.
```sh
jekyll new . --force
```

## 3. Lanyon 테마 적용

가독성이 좋고 깔끔해 간단한 블로그 용으로 Lanyon 테마가 적합하다고 생각해 해당 테마를 적용하였다.
먼저 Lanyon github에서 압축파일을 다운받는다.
그리고 _posts를 제외한 나머지 파일을 Local Repository에 덮어써서 저장한다.
마지막으로 Remote Repository에 적용시킨다.
```sh
git add *
git commit -m 'Lanyon thema'
git push origin main
```

## 4. 결과 확인 및 수정

https://2wodnjs7.github.io/ 에 접속하여 테마가 잘 적용되었는지 확인한다.
그리고 네비게이션 바의 위치를 반대로 옮기고, 그 수를 5개에서 2개로 줄였다.
