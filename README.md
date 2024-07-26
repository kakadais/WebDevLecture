
## 기간
- 2024-07-18 ~ 2024-09-05 (35일/206시간)
- 매주 월,화,수,목,금 (10:00-17:00)

## 강의 목차
- 웹시스템과 웹개발의 이해
- 프로그래밍 세계관
- 자바스크립트 기본
- 데이터전송: 네트워크 프로토콜
- 자바스크립트 활용
- Next.js 개요 및 설치
- HTML 기초
- CSS 기초
- React.js 기초
- MongoDB와 Next.js 연동
- Next.js 추가기능 개발

## 강의 목표
- 스스로 학습을 지속 할 수 있는 상태
- 번아웃을 탈출하고 해 온 공부를 복습한다.

![IT WordCloud](./IT_circle_wordcloud.png)
![AI시대의 학습](https://media.licdn.com/dms/image/D5612AQGvZzUSfk-NnA/article-cover_image-shrink_720_1280/0/1675286537360?e=2147483647&v=beta&t=zsXfMAE9NTIlefG5JxNb-RGpvcMiQFd6ESJ8yjLR290)
![더닝-크루거효과](https://understandinginnovation.blog/wp-content/uploads/2015/06/dunning-kruger-0011.jpg)


## 학습 환경 구성

### 1. Visual Studio Code 설치
1. [Visual Studio Code 공식 사이트](https://code.visualstudio.com/)로 이동합니다.
2. 운영 체제에 맞는 설치 파일을 다운로드합니다.
3. 다운로드한 설치 파일을 실행하고 설치를 완료합니다.

### 2. Visual Studio Code에서 프로젝트 열기
1. VSCode를 실행합니다.
2. `파일` > `열기`를 선택하고, 작업할 폴더를 선택합니다.

### 3. 필수 확장 기능 설치
1. VSCode에서 왼쪽 사이드바에 있는 `Extensions` 아이콘을 클릭합니다 (사이드바의 네 번째 아이콘).
2. 다음 확장 기능을 검색하여 설치합니다:
   - **ESLint**: 코드 린팅을 도와줍니다.
   - **Prettier - Code formatter**: 코드 포맷팅을 도와줍니다.
   - **JavaScript (ES6) code snippets**: 자주 사용하는 JavaScript 코드 조각을 제공합니다.
   - **Next.js snippets**: Next.js와 관련된 코드 조각을 제공합니다.
   - **Tailwind CSS IntelliSense**: Tailwind CSS를 사용하는 경우 유용한 자동 완성 기능을 제공합니다.

### 4. 기본 설정
1. VSCode의 왼쪽 하단에 있는 톱니바퀴 아이콘(설정)을 클릭하고 `설정`을 선택합니다.
2. 오른쪽 상단의 `파일 아이콘`을 클릭하고 `settings.json` 파일을 엽니다.
3. 아래 설정을 추가하여 VSCode의 기본 설정을 구성합니다:
   ```json
   {
     "editor.formatOnSave": true,
     "editor.codeActionsOnSave": {
       "source.fixAll.eslint": true
     },
     "eslint.validate": [
       "javascript",
       "javascriptreact",
       "typescript",
       "typescriptreact"
     ]
   }
   ```

### 5. ESLint 및 Prettier 설정 파일 생성
1. 프로젝트 루트에 `.eslintrc.json` 파일을 생성하고 다음 내용을 추가합니다:
   ```json
   {
     "extends": "next/core-web-vitals"
   }
   ```
2. 프로젝트 루트에 `.prettierrc` 파일을 생성하고 다음 내용을 추가합니다:
   ```json
   {
     "semi": true,
     "singleQuote": true,
     "printWidth": 80,
     "tabWidth": 2,
     "trailingComma": "es5",
     "endOfLine": "auto"
   }
   ```

### 6. 코드 작성 및 실행
1. VSCode에서 새로운 파일을 생성하거나 기존 파일을 열어 코드를 작성합니다.
2. 파일을 저장할 때마다 자동으로 포맷팅되고 린팅됩니다.

이제 VSCode에서 Next.js 프로젝트를 설정하고 개발을 시작할 준비가 완료되었습니다. 필요한 Node.js 설치와 프로젝트 생성은 별도로 진행해야 합니다.
