## 📝 OTT 플랫폼 통합 DB (2人 프로젝트)
##### TMDB API, PostgreSQL, Python을 이용한 OTT 플랫폼 통합 DB 구축

----
## 👥 팀 소개

| 이름   | 학번     |
| :----: | :------: |
| 김*현  | ****1677 |
| 조*우  | ****1716 |
----

## 🛠 Tools and Technologies
![Python](https://img.shields.io/badge/Python-%233776AB.svg?&style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-%2331575F.svg?&style=for-the-badge&logo=postgresql&logoColor=white)

----

## 🔑 핵심 기능

- TMDB API를 활용해 영화, TV 프로그램, 인물 데이터를 수집하여 PostgreSQL에 통합 데이터베이스 구축
- 사용자 선호에 따른 플랫폼별 콘텐츠 수량 분석 및 맞춤 검색 기능 제공
- 특정 OTT 플랫폼과 장르를 지정해 콘텐츠를 검색할 수 있는 기능 구현
- ER 다이어그램 및 릴레이션 스키마 설계를 통해 데이터 구조 최적화

----

## 🔍 담당 업무
- TMDB API를 활용한 데이터 수집 및 정제
- 데이터 자동 수집을 위한 Python 스크립트 작성
- ER 다이어그램 및 릴레이션 스키마 설계

----

## 📅 프로젝트 기간
2023.05

----
## 🎞 쿼리문 / 쿼리 결과물 예시
#### 1. 콘텐츠별 지원 플랫폼 검색
![image](https://github.com/user-attachments/assets/f285b528-ee96-417c-96b9-b4990bfe5728)

찾고자하는 콘텐츠의 제목을 입력 시, 해당 콘텐츠를 제공하는 OTT 플랫폼의 종류를 알 수 있습니다.

---
#### 2. 플랫폼별 지원 콘텐츠 검색

![image](https://github.com/user-attachments/assets/52911573-4e4f-4e78-a850-433c00541fcc)

‘wavve’ 플랫폼에서 제공하는 ‘공포'와 ‘스릴러' 장르의 영화를 검색해볼 수 있습니다.

---
#### 3. 선호 콘텐츠 기반 OTT 플랫폼 추천

![image](https://github.com/user-attachments/assets/456b845d-96bc-42fe-8422-3734aa379018)

‘lion’ 사용자의 선호 콘텐츠를 검색하고, 해당 서브쿼리의 결과를 바탕으로 해당 콘텐츠들을 지원하는 플랫폼들의  ‘플랫폼번호'로 GROUP BY를 수행한 뒤, 플랫폼 별 COUNT를 계산합니다. 결과적으로 어떤 플랫폼이 내가 선호하는 컨텐츠들을 가장 많이 제공하는지 알 수 있습니다.

---
#### 4. 선호 장르 기반 콘텐츠 추천

![image](https://github.com/user-attachments/assets/c7227449-2abf-45dc-904d-9a8c0e007def)

‘horse’ 사용자의 선호 장르를 검색하고, 해당 서브쿼리의 결과를 바탕으로 선호 장르에 속하는 콘텐츠를 ‘인기도’ 순으로 보여줄 수 있습니다.

----
## 🛠 E-R 다이어그램
![image](https://github.com/user-attachments/assets/b153f469-14f4-4d30-8b5e-cc6b7ce5d59d)

----
## 🛠 릴레이션 스키마
![image](https://github.com/user-attachments/assets/cc53241c-e103-4cf4-85f1-01b6a15ef411)

###### 외래키는 밑줄로 표시되었습니다.

----
## 📂 데이터 예시
![image](https://github.com/user-attachments/assets/317e3a2a-ee17-424f-b814-60d28df34f74)

