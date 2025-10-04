# 시민의 소리 siso
siso는 국회의원의 발의안, 뉴스 등 활동을 확인하고, 평가를 작성해 시민들과 의견을 나누기 위한 서비스입니다. 

# 기능 목록 
#### 국회의원 정보 
- 국회의원 소속 정당, 이미지, 당선이력 등 프로필 정보 제공
- 국회의원 발의안 요약 내용, 링크 등 제공
- 국회의원 국회뉴스 제목, 링크 등 제공

#### 평가
- 국회의원 평점 기능 제공
- 국회의원 좋아요/싫어요 기능 제공
- 국회의원 평가 작성 기능 제공
- 국회의원 평가에 대해 좋아요/싫어요 기능 제공

#### 로그인
- 카카오, 네이버 로그인 기능 제공

# 서비스 구성

<img width="756" height="591" alt="siso_시스템_구성도 drawio" src="https://github.com/user-attachments/assets/0b3d114c-4e73-4319-b291-89217571863f" />

- spring scheduler 를 통해 주기적으로 국회 api로 필요 정보 업데이트 
- 발의안은 perplexity api 를 호출해 내용 요약
- jenkins 를 통한 ci/cd 자동화 (main 브랜치 push 시 자동 빌드/배포)
- 카카오, 네이버 로그인 api 로 각각 로그인 기능 제공

# 팀원
- FRONTEND [조다한](https://github.com/orgs/gb-siso/people/JODAHANI)
- BACKEND [장지담](https://github.com/jd99iam)
