## 📝 OTT 플랫폼 통합 DB
##### TMDB API, MySQL, Python을 이용한 OTT 플랫폼 통합 DB 구축

----
## 👥 팀 소개

|   |
| :------------: |
| 김승현|
|  ****1677 |
||

| :------------: |
| 조성우 |
|  ****1716 |

----

## 🛠 Tools and Technologies
![Python](https://img.shields.io/badge/Python-%233776AB.svg?&style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-%234479A1.svg?&style=for-the-badge&logo=mysql&logoColor=white)

----

## 📅 프로젝트 기간
2023.05

----
## ⚙ 프로젝트 개발 배경
최근 TV 프로그램, 영화, 다큐멘터리, 애니메이션 등 다양한 콘텐츠가 등장하고, 이를 소비하는 인구가 증가함에 따라 OTT(Over-the-Top) 서비스의 인기가 크게 높아졌습니다. OTT 서비스는 언제 어디서나 콘텐츠를 다시 시청할 수 있는 편리성을 제공합니다. 현재 다양한 플랫폼에서 OTT 서비스를 제공하고 있으며, 각각의 서비스들이 치열하게 경쟁을 하고 있습니다. 이러한 경쟁에서도 특히, 특정 콘텐츠는 A라는 플랫폼에서만 독점적으로 제공하여 자사의 플랫폼을 이용하도록 유도하고 있습니다. 그러나 이로 인해 소비자는 시청하고자 하는 콘텐츠가 어느 플랫폼에서 제공되는지 확인하기 위해 여러 플랫폼을 일일이 확인해야 하는 번거로움이 있습니다. 또한 각 플랫폼마다 제공하는 콘텐츠를 모아볼 수 있다면 플랫폼 선택에도 도움을 받을 수 있을 것입니다.

이에 따라 저희는 사용자가 쉽고 빠르게 특정 콘텐츠가 어느 플랫폼에서 제공되는지, 또는 특정 플랫폼에서 어떤 콘텐츠를 제공하는지와 같은 정보를 알 수 있도록 돕고자 합니다. 더 나아가 콘텐츠의 상세 정보도 함께 수집하여 사용자가 원하는 콘텐츠를 더욱 정확하게 찾아볼 수 있도록 제공할 것입니다.
 
----
## 🕶 프로젝트의 목적
- 플랫폼-콘텐츠 검색 편의성 제고
 OTT 서비스는 유료로 제공되며, 사용자는 서비스를 이용하기 위해 구독 비용을 지불해야 합니다. 하지만 넷플릭스, 디즈니 플러스, 왓챠, 웨이브 등 각 플랫폼은 독립적인 콘텐츠 라이브러리를 보유하고 있습니다. 이로 인해 사용자는 원하는 콘텐츠를 찾기 위해 여러 플랫폼을 번갈아가며 검색해야 하는 불편함을 겪고 있습니다. 저희 프로젝트의 목적 중 하나는 사용자가 콘텐츠를 검색하면 어느 플랫폼에 해당 콘텐츠가 존재하는지, 또 플랫폼에 따라 제공하는 콘텐츠는 무엇이 있는지를 빠르게 알 수 있는 DB 시스템을 구축하는 것입니다.

- 콘텐츠와 인물 정보 제공
 본 프로젝트에서는 콘텐츠와 배우 및 감독의 상세 정보를 수집하여 제공합니다. 이는 사용자가 원하는 콘텐츠의 장르, 출연 배우, 감독, 개요, 인기도 등을 확인할 수 있게 해줍니다. 또한 인물(배우, 감독) 정보도 수집함에 따라 콘텐츠와 연관된 정보를 정확하고 상세하게 제공하여 콘텐츠 선택에 도움을 줄 수 있습니다.

- 맞춤화된 콘텐츠 추천
 사용자의 편의성을 높이는 것뿐만 아니라, 사용자에게 맞춤화된 콘텐츠를 추천하는 기능을 제공합니다. 회원가입 시 사용자는 선호하는 장르와 선호하는 콘텐츠를 선택할 수 있습니다. 이 정보를 활용하여 사용자에게 맞춤화된 콘텐츠 추천을 제공할 수 있습니다. 이를 통해 사용자는 자신의 취향에 맞는 콘텐츠를 더욱 쉽게 찾아볼 수 있으며, 새로운 콘텐츠를 발견하는 기회를 얻을 수 있습니다.

----
## 🕶 데이터 수집 및 확보 방안
The Movie Database(TMDB)는 영화, TV 프로그램에 대한 다양한 정보를 제공하는 웹사이트입니다. 이 웹사이트에서는 TMDB API를 제공하는데, 이는 TMDB에서 제공하는 개방형 API로 전 세계 언어를 지원하며 오픈소스로서 영화, TV 프로그램, 배우, 감독 등의 다양한 정보를 수집하기 용이하기 때문에 TMDB API를 활용하여 본 프로젝트에 필요한 데이터를 수집하기로 하였습니다. https://developer.themoviedb.org에서 TMDB API에 대한 정보를 확인할 수 있습니다. API를 활용하면 본 프로젝트에 필요한 영화, TV 프로그램과 관련된 다양한 데이터를 확보할 수 있습니다. TMDB 웹사이트에 가입을 하고 API 키를 확보한 뒤, TMDB API 활용을 위한 준비를 하였습니다.

본 프로젝트에서는 Google Colab과 Python을 활용합니다. Colab을 통한 API 요청은 한국에서의 API 응답 시간을 약 2배 정도 줄여주었습니다. 약 40시간 동안 API 요청과 응답이 이루어졌으며, Python을 활용해 영화, 인물, 플랫폼 등의 데이터를 json 형태로 수집하여 필요한 데이터를 csv 파일로 가공하였습니다. 우선 영화와 TV 프로그램을 약 38,000편, 약 7,000편를 수집하였으며, 이를 구분하기 위해 ‘콘텐츠구분’ 속성을 추가하고, 콘텐츠 릴레이션으로 합쳤습니다. 그리고 ‘콘텐츠'와 연관된 데이터인 인물 약 56,000명의 데이터와 장르, 플랫폼 데이터 등의 정보를 수집함과 동시에 각 릴레이션들의 M:N 조건을 충족시키기 위해 매핑 테이블 csv 파일을 생성하였습니다. 사용자 정보는 임의의 값으로 100개의 더미 데이터를 만들어 사용하였습니다. 각 사용자의 선호 장르와 선호 컨텐츠 데이터 또한 임의로 생성하였습니다.

----
## 🕶 기대효과
기존에는 각각의 플랫폼을 가입하며 원하는 콘텐츠를 검색해야했지만, OTT 플랫폼 통합 DB를 통해 하나의 플랫폼에서 모든 콘텐츠를 검색할 수 있게 됩니다. 이로써 사용자의 편의성을 향상시킬 수 있으며, 여러 플랫폼을 개별적으로 접속할 필요가 없으므로 사용자의 시간과 노력을 절약할 수 있습니다. 보다 다양한 콘텐츠를 탐색할 수 있게 됩니다. 하나의 플랫폼을 사용한다면, 그곳에서 제공하는 제한된 범위의 콘텐츠만 발견하게 됩니다. OTT 플랫폼 통합 DB를 활용한다면 다양한 플랫폼에서 제공하는 콘텐츠를 발견할 수 있어 새로운 콘텐츠를 발견하고 다양한 장르와 테마를 고르는데 도움이 될 것입니다. 또한 보다 개인화된 추천 서비스를 제공할 수 있을 것입니다. 기존 OTT 서비스에서는 다른 사람들의 즐겨찾기 리스트를 통해 추천을 해주었으나, 사용자의 성별, 나이 등의 정보를 적극 활용해 추천 시스템을 제공한다면 사용자에게 맞춤화된 콘텐츠를 제공할 수 있게 될 것입니다. 더불어, 콘텐츠의 인기도를 활용하여 대중들에게 인기가 있는, 재미가 어느 정도 보장된 콘텐츠들을 추천할 수 있게 될 것입니다. 마지막으로, OTT 플랫폼 통합 DB를 제공함으로써 사용자들은 기존 OTT 플랫폼보다 더 편리하고 포괄적인 서비스를 제공할 수 있게 되어, OTT 서비스의 시장 경쟁력을 강화할 수 있게 될 것입니다.

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
