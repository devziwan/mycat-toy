# 🐱 MyCat - 고양이 이미지 랜덤 뷰어 iOS 앱

**MyCat**은 주변 지인의 요청으로 시작한 개인 학습용 iOS 앱입니다.  
다양한 고양이 이미지를 외부 API에서 받아와 인스타그램 릴스 스타일 UI로 랜덤하게 보여주며, 즐겨찾기와 사용자 이미지 업로드 기능을 포함합니다.  
네트워크 통신은 URLSession부터 Alamofire, 그리고 Router 패턴까지 점진적으로 적용하며 실무에 가까운 코드 구조를 익혔습니다.

## 프로젝트 개요

- 고양이 이미지를 외부 API에서 받아와 인스타그램 릴스(Reels) 스타일 UI로 랜덤하게 보여줍니다.  
- 사용자는 이미지 즐겨찾기, 로컬 저장, 직접 이미지 선택 및 업로드가 가능합니다.  
- URLSession부터 Alamofire, Alamofire Router 패턴까지 네트워크 통신 구조를 단계적으로 개선하며 실무에 적합한 코드 작성법을 학습했습니다.

## 개발 인원

- 1인 개인 프로젝트 (기획부터 설계, 개발 전 과정 수행)

## 프로젝트 버전별 저장소

| 버전               | 설명                    | 링크 및 사용 기술                                   |
|--------------------|-------------------------|----------------------------------------------------|
| URLSession         | 네이티브 URLSession 기반 구현 | 🔗 [바로가기](https://github.com/devziwan/mycat-urlsession-toy)  Swift, URLSession |
| Alamofire          | Alamofire 도입 개선 버전    | 🔗 [바로가기](https://github.com/devziwan/mycat-alamofire-toy)  Swift, Alamofire  |
| Alamofire + Router | Router 패턴 활용 최종 구조   | 🔗 [바로가기](https://github.com/devziwan/catapp-alamofire-router-toy) Swift, Alamofire, Router 패턴 |

> 각 저장소에서는 네트워크 구조 발전 과정을 확인할 수 있습니다.

## 주요 기능

- **랜덤 고양이 이미지 보기**  
  API에서 받아온 고양이 이미지를 인스타그램 릴스 스타일의 UI로 랜덤하게 표시합니다.  
  *(릴스 UI란 짧은 영상이나 이미지를 세로로 스와이프하며 넘기는 방식의 사용자 인터페이스입니다.)*

- **앨범에서 고양이 사진 선택 및 업로드**  
  사용자가 사진 앱에서 직접 고양이 이미지를 선택해 앱에 업로드할 수 있습니다.

- **즐겨찾기 및 로컬 저장 기능**  
  마음에 드는 고양이 이미지를 즐겨찾기에 추가하고, 로컬에 저장하여 관리할 수 있습니다.

## 스크린샷 및 영상
추후 업데이트 예정

## 네트워크 통신 개선 과정

### 1. URLSession 기반 초기 구현
- iOS 기본 네트워크 프레임워크인 `URLSession`을 사용해 직접 요청, 응답 및 JSON 파싱 구현  
- 네트워크 기본 구조를 이해하는 데 중점  
- 코드 중복과 복잡성 문제 존재

### 2. Alamofire 적용
- `Alamofire` 도입으로 네트워크 요청과 에러 처리 간소화  
- 코드 가독성과 유지보수성 향상

### 3. Alamofire + Router 패턴 구조 적용
- API 요청별로 라우터를 분리하는 구조 도입  
- 모듈화 및 확장성이 뛰어난 네트워크 아키텍처 완성  
- 실무에 적합한 네트워크 처리 방식 경험

## 실행 화면

| 고양이 랜덤 이미지 | 고양이 즐겨찾기 추가 + 목록 확인 | 내 앨범에서 고양이 이미지 추가 + 보관 장소 이동| 고양이 이미지 멀티 삭제 | 즐겨찾기 삭제 |
|---|---|---|---|---|
| <p>앱 실행 시 랜덤으로 고양이 이미지를 표시합니다.</p><img src="https://github.com/user-attachments/assets/899c507b-09dc-4cdc-b9ed-84e5e312ee30" width="250"/> | <p>릴스 화면에서 상세페이지 들어가 즐겨찾기 버튼 클릭 후<br>목록에 자동 추가됩니다.</p><img src="https://github.com/user-attachments/assets/e84c21a4-878f-4bb0-a2c1-d41e413b5f1f" width="250"/>  | <p>내 앨범에서 기기 사진을 선택하여<br>고양이 이미지를 업로드합니다.</p><img src="https://github.com/user-attachments/assets/55dbf9a9-8cf6-4a79-bb6e-916c0bc4eb59" width="250"/> | <p>여러 고양이 이미지를 선택 후<br>삭제 버튼을 눌러 한 번에 제거합니다.</p><img src="https://github.com/user-attachments/assets/2121fede-e27a-450b-b248-7b765fb019ef" width="250"/> | <p>즐겨찾기 목록에서 항목을 선택해<br>즐겨찾기를 해제합니다.</p><img src="https://github.com/user-attachments/assets/bbdde8af-4fdf-44df-b8f0-c16f985c6f34" width="250"/> |















