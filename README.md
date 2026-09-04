# 마이볼로그 제품 데이터

마이볼로그 Android 앱이 수동으로 제품 DB 업데이트를 확인할 때 내려받는 공개 카탈로그입니다.

- 공개 파일: `catalog.json`
- 개인 장비, 지공 정보, 보관장소, 백업 파일은 이 저장소에 포함하지 않습니다.
- 앱은 `schemaVersion`, 제품 ID 중복, 한글 검색 별칭 및 출시일 데이터 연결을 검사한 뒤에만 새 카탈로그를 적용합니다.

## 업데이트 방법

앱 프로젝트에서 제품 데이터를 수정한 뒤 `tool/generate_catalog_json.dart`를 실행합니다. 생성된 `data/catalog.json`을 이 저장소의 `catalog.json`으로 교체하고, 검증 후 `main` 브랜치에 올립니다.
