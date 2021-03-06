# 나무위키-오픈나무 데이터 컨버터
나무위키가 배포하는 JSON파일을 오픈나무에 맞게 컨버팅하는 스크립트입니다.


>윈도우 환경에서 정상적으로 동작하지 않습니다.

>또한 생각 없이 만들어서 메모리 엄청 잡아먹습니다. (12GB 이상), 추후 바꿀 예정입니다.

>오픈나무의 구조상 문제 때문에 리눅스 환경에서는 일정 개수 이상 문서를 변환할 수 없습니다. (아이노드 제한) 이것은 오픈나무의 문제이며 오픈나무가 해결해야 합니다.

## 되는 것
* 나무위키의 JSON파일을 읽어서 파이썬 dict형식으로 변환하기
* 사전형으로 변환한 파일을 읽어서 오픈나무가 받아들일 수 있는 형식으로 변환하기
* 문서 편집자의 종류 구별하기 (리그베다 위키,나무위키,익명)


## 안되는 것
* 나무위키에서의 편집 로그 반영 (JSON 파일에 해당 데이터가 없습니다)
* 윈도우 환경에서의 실행 (파이썬 3.6 이상에서는 가능합니다) 

## Todo
* IP주소 구분 방식 바꾸기
* 오픈나무 구조변경 대응
* JSON 파일을 한줄한줄 읽어서 단계적으로 처리하는 구조로 변경

## 의존성
* 파이썬 3.0 이상

## 사용법
1. 빈 디텍토리를 하나 만듭니다.
2. 그 디텍토리에 나무위키 JSON파일의 이름을 namuwikidata.json으로 바꾸고 집어 넣습니다.
3. 그 디텍토리에서 파이썬 스크립트를 실행시킵니다.
4. 출력된 결과물들을 오픈나무 폴더로 옮깁니다.
