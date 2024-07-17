## 소개
- 진정원
	- 건국대 컴퓨터공학 / 상명대 컴퓨터공학 박사
	- 현 (주)코디지 대표
	- 한국정보통신 연구원
	- KT데이터시스템 연구원
- 주요 프로젝트
	- 우리카드/CJ오쇼핑 홈페이지 챗봇/상담톡 시스템
	- 라이나생명 전성기 프로젝트 총괄 개발
	- 제로페이(한국간편결제진흥원) 백오피스 및 Z-Map iOS/Android 앱 시스템 개발
- 주요 강의
	- 교육기관
		- 인하공대 / 서울여대 / 가톨릭대 / 상명대 / 마에스터고
	- 공공/기업/기관
		- 인터넷진흥원 / 한국정보과학회 / KOSTA / KEA / LS산전 / 한전 / 남부여성발전센터

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
- 자바스크립트 언어로 풀스택 개발을 수행할 수 있도록 한다.
- 프로그래밍의 기초와 제반 사항을 학습한다.
- 개발 환경 전반을 이해하여 향후 스스로 학습할 수 있는 상태를 도모 한다.
- 종합적인 이해를 통해 독립적으로 프로젝트를 진행할 수 있는 역량을 키운다.

![IT WordCloud](./IT_circle_wordcloud.png)
![AI시대의 학습](https://media.licdn.com/dms/image/D5612AQGvZzUSfk-NnA/article-cover_image-shrink_720_1280/0/1675286537360?e=2147483647&v=beta&t=zsXfMAE9NTIlefG5JxNb-RGpvcMiQFd6ESJ8yjLR290)
![더닝-크루거효과](https://understandinginnovation.blog/wp-content/uploads/2015/06/dunning-kruger-0011.jpg)


## 학습 환경 구축

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