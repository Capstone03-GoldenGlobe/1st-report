# Team-Info
| (1) 과제명 | GoldenGlobe : 시니어를 위한 LLM과 RAG 기반 맞춤형 여행 챗봇, 체크리스트 서비스
|:---  |---  |
| (2) 팀 번호 / 팀 이름 | 03-이대뎅김 |
| (3) 팀 구성원 | 김근주 (2071006): 리더, 백엔드, AI, 배포 <br> 김현수 (2073100): 팀원, 프론트엔드, 와이어프레임 및 디자인  </br> 원재영 (2176225): 팀원, 백엔드, AI	|
| (4) 팀 지도교수 | 이형준 교수님 |
| (5) 팀 멘토 | 김동수 / CTO / 엘핀 |
| (6) 과제 분류 | 산학과제 |
| (7) 과제 키워드 | 여행, 시니어, 챗봇, RAG, LLM  |
| (8) 과제 내용 요약 | 시니어와, 시니어를 가족 구성원으로 둔 나머지 가족들의 효율적인 여행 준비를 돕는 서비스입니다. <br><br> 챗봇 기능을 통해 시니어가 주도적으로 여행을 파악하고 준비할 수 있도록 돕고,<br>여행지 맞춤 생성형 공유 체크리스트 기능을 통해 여행 준비의 효율성을 증대시킵니다. |

# Project-Summary
| 항목 | 내용 |
|:---  |---  |
| (1) 문제 정의 | **[본 과제를 통하여 해결 / 완화하고자 하는 문제]** <br>- 시니어 개인 혹은 시니어와 함께하는 가족이 여행을 준비할 때 겪는 여러 어려움<br><br> 1. **시니어** : 가족 여행, 해외 여행, 패키지 여행을 가고자 하는 시니어<br>	- 검색 시간 소요 : 인터넷에 익숙하지 않아 여행에 필요한 정보에 접근하는 데 시간이 많이 소요됨. 여행 관련 문서에서 필요한 정보를 찾는데 시간이 소요됨.<br> - 정보 부족 : 세부 일정을 확인하기 위해 가족의 답변을 기다리거나, 전화 상담이나 Q&A 게시판을 이용해야 하는 등 여러 절차를 거쳐야 함.<br> <br>2. **가족** : 시니어와 함께하는 여행을 떠나려는, 혹은 여행을 보내드리려는 가족(자녀 입장)<br>- 정보제공의 어려움 : 시니어와 함께 여행을 가거나 시니어의 여행을 도울 때 추가적인 설명이나 정보를 제공해야 함<br> - 준비물 공유 : 시니어와 함께 여행 준비물 목록을 한번에 공유하고 확인할 수 있는 플랫폼이 없어 불편함.<br><br>실제로 시니어와의 여행 준비 과정에서 겪는 어려움을 주제로 설문조사를 진행한 결과, <br> - 여행 관련 문서를 정리하고, 관련 정보를 찾는데 어려움을 겪었다는 응답 : **89.3%** <br>- 그 외에, 정보 제공의 어려움을 겪었다는 응답 : **48%** <br> - 준비물 준비 및 확인으로 어려움을 겪었다는 응답 **41.3%** <br>
| (2) 기존연구와의 비교 | **[유사한 과제 / 연구 / 서비스 / 시스템]** <br> - **아고다** : 고정된 키워드(ex.'캐쉬백 리워드','Acoda Cash')로만 문의 가능<br> - **익스피디아**  : 챗봇 파일 첨부 지원X -> 사용자 개개인 맞춤형 답변 제공 불가 <br> - **스카이 스캐너** : 챗봇 서비스 제공X, QnA 문의를 남기는 서비스만 존재<br> - **하나투어** : ‘AI 채팅상담 서비스'가 있으나 최신 정보 답변 X <br> - **트리플** : 챗봇 서비스 제공X, 공유 체크리스트가 있으나 기본 템플릿만 제공 <br><br><br> **[본 과제가 유사 과제에 비해 갖는 장점]** <br> **공통** : 챗봇 서비스와 체크리스트 서비스 동시에 제공한다. <br> <br> 1. **챗봇** <br> - 일반적 답변이 아닌, 관련 PDF를 기반으로 한 사용자 맞춤형 답변 제공 <br> - 고정된 키워드가 아닌, 자유로운 의사소통 기반 <br> - RAG를 기반으로 답변하기에, 거짓 없는 정확한 답변 제공 <br> <br> 2. **체크리스트** <br> - 기본 템플릿이 아닌, 여행지 날씨와 관련 PDF를 기반으로 한 맞춤형 체크리스트 제안
| (3) 제안 내용 | 시니어와 그 가족이 주도적으로 여행을 즐기고, 준비 과정을 간편하게 관리할 수 있도록 돕는다. <br> <br> **공통** : 가족 단위의 여행에 따르는 소통 부담과 피로를 덜어 더 만족감 높은 여행을 경험할 수 있다. <br><br>1. **시니어** <br> - RAG,LLM을 활용한 챗봇을 활용해 여행할 때 필요한 정보 검색 시간을 줄이고 보다 정확한 답변을 제공받는다. <br> - 체크리스트 제안 기능과 공유 체크리스트 기능을 통해 준비물 준비 시간을 줄이고, 효율적인 준비를 할 수 있다. <br><br> 2. **시니어의 가족** <br> - 체크리스트 기능을 통해 여행 준비물을 한 페이지에서 편리하게 관리할 수 있다. <br> 
| (4) 기대효과 및 의의 | - 시니어가 주도적으로 여행에 참여할 수 있다.<br>- 시니어는 챗봇을 통해 검색시간을 줄이고, 보다 정확한 답변을 제공받을 수 있다. <br>- 시니어가 여행하고자 하는 나라의 상황(날씨, 관광지, 음식 등)에 적합한 준비물을 챙겨 예상하지 못한 상황을 대비할 수 있게 된다.<br>- 시니어와 가족은 체크리스트를 통해 여행 준비물을 한꺼번에 편리하게 관리할 수 있다.<br>- 가족 단위의 여행에 따르는 소통 부담과 피로를 덜어 더 만족감 높은 여행 경험을 제공할 수 있다.
| (5) 주요 기능 리스트 | 1. '챗봇' 기능<br>- LLM, RAG를 활용하여 pdf 기반 챗봇을 생성한다.<br>- 여행 전자 영수증, 패키지 화면 pdf, 액티비티 예약 캡쳐본 등 여행 관련 문서를 저장해 두면 언제든지 해당 문서의 내용을 추출하여 정확한 질의응답을 할 수 있다.<br><br>2. '체크리스트' 기능<br>- 날씨 api와 생성형 ai를 사용해, 여행지의 특성에 맞는 맞춤형 준비물을 기본적으로 생성한다.<br>- 사용자가 업로드한 pdf 분석을 통한 준비물을 추천한다.<br>- 가족들이 함께 체크리스트를 작성하여, 시니어가 꼼꼼하게 준비물을 챙길 수 있도록 돕는다.<br>- 체크리스트에서, 가족들이 시니어에게 메모를 남겨 중요한 부분을 다시 한 번 강조할 수 있다. 


<br>
 
# Project-Design
| 항목 | 내용 |
|:---  |---  |
| (1) 요구사항 정의 | - 요구사항 정의서 (기획의 전반적인 설명)<img width="800" alt="기능명세서1" src="./document/기능명세서1.png"><br><img width="800" alt="기능명세서2" src="./document/기능명세서2.png"><br><img width="800" alt="기능명세서3" src="./document/기능명세서3.png"><br><br>- ui 디자인 (프론트의 전반적인 설명)<br><img width="500" alt="디자인1" src="./document/디자인1.png"><br><img width="500" alt="디자인2" src="./document/디자인2.png"><br><img width="800" alt="디자인3" src="./document/디자인3.png"><br><br>- ER 다이어그램 (백앤드의 전반적인 설명)<br><img width="800" alt="ERD" src="./document/ERD.png">
| (2) 전체 시스템 구성 | <img width="1316" alt="SW 구조도" src="./document/시스템구성도.png">  <br> **CLIENT** <br> - Vercel : 서버리스 플랫폼으로 프론트엔드 애플리케이션을 배포하고 관리 <br> - React : 사용자가 입력한 데이터를 서버로 전송, 서버에서 받은 응답을 화면에 표시하여 시니어에 최적화된 UI 제공 <br> - Axios : 서버와 프론트엔드 간 요청 처리 <br> <br> **SERVER** <br> - Spring Boot : 프론트 요청에 따라 DB에 데이터를 저장하거나 필요한 데이터를 찾아서 응답 <br> - Flask : 프론트에서 받은 사용자의 질문을 토대로 챗봇 답변 생성 <br> - Docker : Spring Boot, Flask 서버 컨테이너화 <br> - EC2 : Docker로 패키징된 애플리케이션 호스팅 <br> - GithubActions : 코드 변경 시 배포 자동화 <br> <br> **AI** <br> - PyPdf2 : PDF 텍스트 인식<br> - LangChain : 텍스트 임베딩, 벡터화 <br> - OpenAI : 챗봇 답변 생성, 체크리스트 제안
| (3) 진척도 및 검증내역 | _1학기 종료 이후 주제를 바꿔서 스타트 단계에서 검증한 내용이 없습니다._ <br><br>**전체 진척도 : 60%**<br><br> 1. **프론트** (50%) <br> - 구현 완료 : 퍼블리싱, api 연결(로그인, 메인, 여행지 추가, 챗봇) <br> - 미구현 : api 연결(체크리스트, 마이페이지, 회원가입) <br><br> 2. **백** (70%) <br> - 구현 완료 : ERD, API (유저, 여행지, 체크리스트, 챗봇, 공유, PDF) <br> - 미구현 : 체크리스트 제안, 알림 API<br><br> 3. **AI** (50%) <br> - 구현 완료 : 챗봇 AI 모델 <br> - 미구현 : 체크리스트 제안 기능 구현 중(프롬프트 진행 중) <br><br> 4. **시스템 통합 및 테스트** (70%) <br> - 구현 완료 : Spring Boot 배포 및 CI/CD 구축, Flask 배포, 프론트 배포 <br> - 미구현 : Flask CI/CD 구축, 테스트
| (4) 기타 |  |

<br>
