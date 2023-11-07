# 보고서
# USED
![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![Tensorflow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
# Tested On
![12400](https://img.shields.io/badge/Intel-Core_i5_12400-0071C5?style=for-the-badge&logo=intel&logoColor=white
)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

## 서론
컴퓨터를 이용한 정보 처리가 점차 증가하고 있으며, 동시에 과거의 여러 가지 기록물을 디지털화하는 과정에서 효율성을 추구하기 위해 OCR 등의 방식을 이용하고 있다. OCR 기술은 현재까지 20년 이상 사용되었으며, 문서나 이미지만을 인식하던 기술에서 일반적인 사진이나 동영상 속 문자까지도 인식할 수 있는 기술로 발전하고 있다. OCR은 이미지 및 문서 처리 업무를 자동화하여 효율 극대화 및 비용 절감에 효과적이며, 특히 모바일 사용이 대중화되며 처리해야 할 이미지가 모바일 이미지로 바뀌고 있어 그 필요성이 점차 높아지고 있다. 하지만, 기존의 OCR의 경우는 인공지능을 활용하지 않아 그 처리속도와 정확성이 매우 낮으며, 이러한 문제점을 해결하기 위해 OCR과 인공지능을 접목하고자 하였다.
## 연구 동기 및 목적
여러 텍스트 인식 프로그램들을 살펴본 결과, 교과서나 학교 교과 수업 유인물 등을 디지털 문서화하면 편리할 것 같아 이미지를 통해 한글을 디지털화하는 프로젝트를 진행하고자 하였다. 또한, OCR 기술을 딥러닝과 접목하여 기존 OCR 대비 높은 효율성을 달성하고자 하였다. 기존 OCR의 구조는 영상을 이진화하고, 문자 영역을 검출한 후, 라인 또는 단어 단위로 추출하여 문자를 하나씩 인식하고 결합하는 방식을 사용한다. 하지만, 딥러닝을 이용해 OCR을 구현하면 기존과는 달리 각 단계에서 인공지능이 작용하여 높은 품질과 상대적으로 적은 양의 데이터로도 충분한 정확성을 얻을 수 있을 것으로 기대된다.
## 이론적 배경
* GPU: 그래픽 처리 장치(Graphic Processing Unit)의 약자로, 단순 연산 위주의 딥러닝 작업에서 고성능을 발휘한다. CPU에 비해 단일 코어의 성능은 낮지만, 압도적으로 많은 코어의 개수를 보유하고 있어 딥러닝 등에서 CPU 대비 높은 성능을 보여준다.
* OCR: 광학식 문자 인식(Optical Character Recognition)의 약자로, 종이 등지에 적혀 있는 활자를 디지털화하는 기술이다.
* 머신 러닝: 인공지능 연구의 대표적인 방법으로, 사람이 직접 수없이 많은 개수의 규칙을 통해 구현하는 전문가 시스템이 시대의 흐름에 따라 아직 인간이 작동하는 원리조차 파악되지 않은 분야들을 구현하는 프로그램들이 요구되기 시작하자, 방대해진 분야로 인해 스스로 규칙을 형성하게끔 하려는 시도에서 나오게 되었다. 머신 러닝은 통계학과 선형대수학, 수치해석, 이산수학, 미적분학 등을 이용하여 확률분포를 계산하고, 기계 스스로가 규칙을 찾아내도록 하는, 마치 인간이 유아기 때 진행하는 학습과 같은 원리로 기계학습을 하는 것이다.
* 인공신경망: 소프트웨어적으로 인간의 뉴런의 구조를 모방하여 만든 머신 러닝 모델로, 인공지능을 구현하기 위한 기술 중 하나이다. 이는 생물의 신경망, 그 중에서도 특히 인간의 시각, 청각 과정을 모방해 만들어낸 알고리즘이다. 입력층과 출력층 사이에 여러 개의 은닉층을 만들어, 각 층 안에 세포들을 집어넣고, 무작위로 연결한다. 그 이후, 각 세포들은 자신에게 들어온 신호에 가중치를 곱해 총합하며, 그 역치와 비교해 신호를 다음 뉴런으로 전달한다. 이러한 과정이 반복되어 이루어지는 것이 바로 인공신경망이다. 허나, 인간의 뇌는 1000억 개 이상의 세포로 구성되어 있는데, 현재의 기술로는 이렇게 많은 수의 뉴런을 시뮬레이션할 수 없으며, 그 원리조차 점차 인간과는 멀어졌음에도 여전히 효과적인 학습 방법이기에 현재까지도 가장 각광받는 머신 러닝 알고리즘이다.
* 딥 러닝: 딥 러닝(심층 학습)은 머신 러닝 기술인 인공신경망의 방법론으로, 다중 구조의 은닉층으로 네트워크를 연결하는 기법이다. 이는 현대 인공지능 기술의 핵심이자, 미래에 더 빛을 발할 기술 중 하나이다. 딥 러닝은 함수관계에 있는 x와 y가 존재하는 상태에서 x에 대한 함수를 예측할 수 있는 모델이 없을 때 대안으로 사용되는 방법이다.
* MNIST 데이터셋: MNIST 데이터셋은 다양한 화상처리 시스템을 훈련하는데 사용되는 데이터셋으로, 머신 러닝의 훈련 및 테스트에 널리 사용된다. 표준 MNIST 데이터셋은 28*28픽셀의 흑백 그림으로, 0~9의 숫자를 나타내는 손으로 쓴 숫자 이미지로 구성되어 있다.
## 1. 한글에 대한 고찰
### 1-1 한글의 특성
한글은 모아쓰기 방식을 사용하여 자음과 모음이 한 글자에 결합된다. 따라서 특정한 한 글자를 인식하기 위해서는 모든 가능성(초성 19가지, 중성 21가지, 종성 28가지(없는 경우 포함)인 11,172가지)를 따져야 한다. 이는 영어의 경우 단 26가지만 따져도 되는 것과 비교하여 텍스트 인식에 훨씬 불리한 면을 가지고 있다. 그렇기에 인공지능를 활용한 OCR 서비스를 만들 필요성이 크게 존재한다.
### 1-2 OCR이란?
OCR은 Optical Character Recognition의 약자로, 일반적으로 컴퓨터가 이진법 데이터를 폰트를 통해 인간에게 인식시켜주는 것과는 달리, 인간이 작성한 글씨를 분석하여 텍스트 데이터로 치환하는 시스템이다. 이미 존재하는 폰트와 대조하는 방식을 통해 이미지를 인식하기 때문에 고해상도가 필요하게 된다.
### 1-3 구상하게 된 모델
데이터 생성을 위해 한글을 지원하는 폰트를 다운로드한 후, 텐서플로우 모델로 들어가게 된다. 그 후, 그려진 글자가 기존에 학습된 텐서플로우 모델과 안드로이드 텐서플로우 추론 인터페이스로 인식된다. 그 후, 한글 글자들이 문자열로 분류된다.
## 2. 인공지능 학습 방법에 대한 고찰
### 2-1 MNIST 데이터셋
한글 텍스트를 인식하기 위한 방법으로 MNIST와 유사한 방식의 데이터셋을 이용하기로 하였다. MNIST는 손으로 쓴 숫자들을 획이 지나간 부분은 1로, 아닌 부분은 0으로 나타낸 데이터이다. 우리는 이를 한글에 접목하여, 3118개 이상의 한글 MNIST 유형의 64*64픽셀 데이터를 생성하였다. 더 많아진 클래스들을 구분하기 위해 특징을 더 추출하기 위해 3차원 컨볼루션 레이어를 추가하는 방식으로 진행하였다.
<details>
<summary>접기/펼치기</summary>
가
각
간
갇
갈
갉
갊
감
갑
값
갓
갔
강
갖
갗
같
갚
갛
개
객
갠
갤
갬
갭
갯
갰
갱
갸
갹
갼
걀
걋
걍
걔
걘
걜
거
걱
건
걷
걸
걺
검
겁
것
겄
겅
겆
겉
겊
겋
게
겐
겔
겜
겝
겟
겠
겡
겨
격
겪
견
겯
결
겸
겹
겻
겼
경
곁
계
곈
곌
곕
곗
고
곡
곤
곧
골
곪
곬
곯
곰
곱
곳
공
곶
과
곽
관
괄
괆
괌
괍
괏
광
괘
괜
괠
괩
괬
괭
괴
괵
괸
괼
굄
굅
굇
굉
교
굔
굘
굡
굣
구
국
군
굳
굴
굵
굶
굻
굼
굽
굿
궁
궂
궈
궉
권
궐
궜
궝
궤
궷
귀
귁
귄
귈
귐
귑
귓
규
균
귤
그
극
근
귿
글
긁
금
급
긋
긍
긔
기
긱
긴
긷
길
긺
김
깁
깃
깅
깆
깊
까
깍
깎
깐
깔
깖
깜
깝
깟
깠
깡
깥
깨
깩
깬
깰
깸
깹
깻
깼
깽
꺄
꺅
꺌
꺼
꺽
꺾
껀
껄
껌
껍
껏
껐
껑
께
껙
껜
껨
껫
껭
껴
껸
껼
꼇
꼈
꼍
꼐
꼬
꼭
꼰
꼲
꼴
꼼
꼽
꼿
꽁
꽂
꽃
꽈
꽉
꽐
꽜
꽝
꽤
꽥
꽹
꾀
꾄
꾈
꾐
꾑
꾕
꾜
꾸
꾹
꾼
꿀
꿇
꿈
꿉
꿋
꿍
꿎
꿔
꿜
꿨
꿩
꿰
꿱
꿴
꿸
뀀
뀁
뀄
뀌
뀐
뀔
뀜
뀝
뀨
끄
끅
끈
끊
끌
끎
끓
끔
끕
끗
끙
끝
끼
끽
낀
낄
낌
낍
낏
낑
나
낙
낚
난
낟
날
낡
낢
남
납
낫
났
낭
낮
낯
낱
낳
내
낵
낸
낼
냄
냅
냇
냈
냉
냐
냑
냔
냘
냠
냥
너
넉
넋
넌
널
넒
넓
넘
넙
넛
넜
넝
넣
네
넥
넨
넬
넴
넵
넷
넸
넹
녀
녁
년
녈
념
녑
녔
녕
녘
녜
녠
노
녹
논
놀
놂
놈
놉
놋
농
높
놓
놔
놘
놜
놨
뇌
뇐
뇔
뇜
뇝
뇟
뇨
뇩
뇬
뇰
뇹
뇻
뇽
누
눅
눈
눋
눌
눔
눕
눗
눙
눠
눴
눼
뉘
뉜
뉠
뉨
뉩
뉴
뉵
뉼
늄
늅
늉
느
늑
는
늘
늙
늚
늠
늡
늣
능
늦
늪
늬
늰
늴
니
닉
닌
닐
닒
님
닙
닛
닝
닢
다
닥
닦
단
닫
달
닭
닮
닯
닳
담
답
닷
닸
당
닺
닻
닿
대
댁
댄
댈
댐
댑
댓
댔
댕
댜
더
덕
덖
던
덛
덜
덞
덟
덤
덥
덧
덩
덫
덮
데
덱
덴
델
뎀
뎁
뎃
뎄
뎅
뎌
뎐
뎔
뎠
뎡
뎨
뎬
도
독
돈
돋
돌
돎
돐
돔
돕
돗
동
돛
돝
돠
돤
돨
돼
됐
되
된
될
됨
됩
됫
됴
두
둑
둔
둘
둠
둡
둣
둥
둬
뒀
뒈
뒝
뒤
뒨
뒬
뒵
뒷
뒹
듀
듄
듈
듐
듕
드
득
든
듣
들
듦
듬
듭
듯
등
듸
디
딕
딘
딛
딜
딤
딥
딧
딨
딩
딪
따
딱
딴
딸
땀
땁
땃
땄
땅
땋
때
땍
땐
땔
땜
땝
땟
땠
땡
떠
떡
떤
떨
떪
떫
떰
떱
떳
떴
떵
떻
떼
떽
뗀
뗄
뗌
뗍
뗏
뗐
뗑
뗘
뗬
또
똑
똔
똘
똥
똬
똴
뙈
뙤
뙨
뚜
뚝
뚠
뚤
뚫
뚬
뚱
뛔
뛰
뛴
뛸
뜀
뜁
뜅
뜨
뜩
뜬
뜯
뜰
뜸
뜹
뜻
띄
띈
띌
띔
띕
띠
띤
띨
띰
띱
띳
띵
라
락
란
랄
람
랍
랏
랐
랑
랒
랖
랗
래
랙
랜
랠
램
랩
랫
랬
랭
랴
략
랸
럇
량
러
럭
런
럴
럼
럽
럿
렀
렁
렇
레
렉
렌
렐
렘
렙
렛
렝
려
력
련
렬
렴
렵
렷
렸
령
례
롄
롑
롓
로
록
론
롤
롬
롭
롯
롱
롸
롼
뢍
뢨
뢰
뢴
뢸
룀
룁
룃
룅
료
룐
룔
룝
룟
룡
루
룩
룬
룰
룸
룹
룻
룽
뤄
뤘
뤠
뤼
뤽
륀
륄
륌
륏
륑
류
륙
륜
률
륨
륩
륫
륭
르
륵
른
를
름
릅
릇
릉
릊
릍
릎
리
릭
린
릴
림
립
릿
링
마
막
만
많
맏
말
맑
맒
맘
맙
맛
망
맞
맡
맣
매
맥
맨
맬
맴
맵
맷
맸
맹
맺
먀
먁
먈
먕
머
먹
먼
멀
멂
멈
멉
멋
멍
멎
멓
메
멕
멘
멜
멤
멥
멧
멨
멩
며
멱
면
멸
몃
몄
명
몇
몌
모
목
몫
몬
몰
몲
몸
몹
못
몽
뫄
뫈
뫘
뫙
뫼
묀
묄
묍
묏
묑
묘
묜
묠
묩
묫
무
묵
묶
문
묻
물
묽
묾
뭄
뭅
뭇
뭉
뭍
뭏
뭐
뭔
뭘
뭡
뭣
뭬
뮈
뮌
뮐
뮤
뮨
뮬
뮴
뮷
므
믄
믈
믐
믓
미
믹
민
믿
밀
밂
밈
밉
밋
밌
밍
및
밑
바
박
밖
밗
반
받
발
밝
밞
밟
밤
밥
밧
방
밭
배
백
밴
밸
뱀
뱁
뱃
뱄
뱅
뱉
뱌
뱍
뱐
뱝
버
벅
번
벋
벌
벎
범
법
벗
벙
벚
베
벡
벤
벧
벨
벰
벱
벳
벴
벵
벼
벽
변
별
볍
볏
볐
병
볕
볘
볜
보
복
볶
본
볼
봄
봅
봇
봉
봐
봔
봤
봬
뵀
뵈
뵉
뵌
뵐
뵘
뵙
뵤
뵨
부
북
분
붇
불
붉
붊
붐
붑
붓
붕
붙
붚
붜
붤
붰
붸
뷔
뷕
뷘
뷜
뷩
뷰
뷴
뷸
븀
븃
븅
브
븍
븐
블
븜
븝
븟
비
빅
빈
빌
빎
빔
빕
빗
빙
빚
빛
빠
빡
빤
빨
빪
빰
빱
빳
빴
빵
빻
빼
빽
뺀
뺄
뺌
뺍
뺏
뺐
뺑
뺘
뺙
뺨
뻐
뻑
뻔
뻗
뻘
뻠
뻣
뻤
뻥
뻬
뼁
뼈
뼉
뼘
뼙
뼛
뼜
뼝
뽀
뽁
뽄
뽈
뽐
뽑
뽕
뾔
뾰
뿅
뿌
뿍
뿐
뿔
뿜
뿟
뿡
쀼
쁑
쁘
쁜
쁠
쁨
쁩
삐
삑
삔
삘
삠
삡
삣
삥
사
삭
삯
산
삳
살
삵
삶
삼
삽
삿
샀
상
샅
새
색
샌
샐
샘
샙
샛
샜
생
샤
샥
샨
샬
샴
샵
샷
샹
섀
섄
섈
섐
섕
서
석
섞
섟
선
섣
설
섦
섧
섬
섭
섯
섰
성
섶
세
섹
센
셀
셈
셉
셋
셌
셍
셔
셕
션
셜
셤
셥
셧
셨
셩
셰
셴
셸
솅
소
속
솎
손
솔
솖
솜
솝
솟
송
솥
솨
솩
솬
솰
솽
쇄
쇈
쇌
쇔
쇗
쇘
쇠
쇤
쇨
쇰
쇱
쇳
쇼
쇽
숀
숄
숌
숍
숏
숑
수
숙
순
숟
술
숨
숩
숫
숭
숯
숱
숲
숴
쉈
쉐
쉑
쉔
쉘
쉠
쉥
쉬
쉭
쉰
쉴
쉼
쉽
쉿
슁
슈
슉
슐
슘
슛
슝
스
슥
슨
슬
슭
슴
습
슷
승
시
식
신
싣
실
싫
심
십
싯
싱
싶
싸
싹
싻
싼
쌀
쌈
쌉
쌌
쌍
쌓
쌔
쌕
쌘
쌜
쌤
쌥
쌨
쌩
썅
써
썩
썬
썰
썲
썸
썹
썼
썽
쎄
쎈
쎌
쏀
쏘
쏙
쏜
쏟
쏠
쏢
쏨
쏩
쏭
쏴
쏵
쏸
쐈
쐐
쐤
쐬
쐰
쐴
쐼
쐽
쑈
쑤
쑥
쑨
쑬
쑴
쑵
쑹
쒀
쒔
쒜
쒸
쒼
쓩
쓰
쓱
쓴
쓸
쓺
쓿
씀
씁
씌
씐
씔
씜
씨
씩
씬
씰
씸
씹
씻
씽
아
악
안
앉
않
알
앍
앎
앓
암
압
앗
았
앙
앝
앞
애
액
앤
앨
앰
앱
앳
앴
앵
야
약
얀
얄
얇
얌
얍
얏
양
얕
얗
얘
얜
얠
얩
어
억
언
얹
얻
얼
얽
얾
엄
업
없
엇
었
엉
엊
엌
엎
에
엑
엔
엘
엠
엡
엣
엥
여
역
엮
연
열
엶
엷
염
엽
엾
엿
였
영
옅
옆
옇
예
옌
옐
옘
옙
옛
옜
오
옥
온
올
옭
옮
옰
옳
옴
옵
옷
옹
옻
와
왁
완
왈
왐
왑
왓
왔
왕
왜
왝
왠
왬
왯
왱
외
왹
왼
욀
욈
욉
욋
욍
요
욕
욘
욜
욤
욥
욧
용
우
욱
운
울
욹
욺
움
웁
웃
웅
워
웍
원
월
웜
웝
웠
웡
웨
웩
웬
웰
웸
웹
웽
위
윅
윈
윌
윔
윕
윗
윙
유
육
윤
율
윰
윱
윳
융
윷
으
윽
은
을
읊
음
읍
읏
응
읒
읓
읔
읕
읖
읗
의
읜
읠
읨
읫
이
익
인
일
읽
읾
잃
임
입
잇
있
잉
잊
잎
자
작
잔
잖
잗
잘
잚
잠
잡
잣
잤
장
잦
재
잭
잰
잴
잼
잽
잿
쟀
쟁
쟈
쟉
쟌
쟎
쟐
쟘
쟝
쟤
쟨
쟬
저
적
전
절
젊
점
접
젓
정
젖
제
젝
젠
젤
젬
젭
젯
젱
져
젼
졀
졈
졉
졌
졍
졔
조
족
존
졸
졺
좀
좁
좃
종
좆
좇
좋
좌
좍
좔
좝
좟
좡
좨
좼
좽
죄
죈
죌
죔
죕
죗
죙
죠
죡
죤
죵
주
죽
준
줄
줅
줆
줌
줍
줏
중
줘
줬
줴
쥐
쥑
쥔
쥘
쥠
쥡
쥣
쥬
쥰
쥴
쥼
즈
즉
즌
즐
즘
즙
즛
증
지
직
진
짇
질
짊
짐
집
짓
징
짖
짙
짚
짜
짝
짠
짢
짤
짧
짬
짭
짯
짰
짱
째
짹
짼
쨀
쨈
쨉
쨋
쨌
쨍
쨔
쨘
쨩
쩌
쩍
쩐
쩔
쩜
쩝
쩟
쩠
쩡
쩨
쩽
쪄
쪘
쪼
쪽
쫀
쫄
쫌
쫍
쫏
쫑
쫓
쫘
쫙
쫠
쫬
쫴
쬈
쬐
쬔
쬘
쬠
쬡
쭁
쭈
쭉
쭌
쭐
쭘
쭙
쭝
쭤
쭸
쭹
쮜
쮸
쯔
쯤
쯧
쯩
찌
찍
찐
찔
찜
찝
찡
찢
찧
차
착
찬
찮
찰
참
찹
찻
찼
창
찾
채
책
챈
챌
챔
챕
챗
챘
챙
챠
챤
챦
챨
챰
챵
처
척
천
철
첨
첩
첫
첬
청
체
첵
첸
첼
쳄
쳅
쳇
쳉
쳐
쳔
쳤
쳬
쳰
촁
초
촉
촌
촐
촘
촙
촛
총
촤
촨
촬
촹
최
쵠
쵤
쵬
쵭
쵯
쵱
쵸
춈
추
축
춘
출
춤
춥
춧
충
춰
췄
췌
췐
취
췬
췰
췸
췹
췻
췽
츄
츈
츌
츔
츙
츠
측
츤
츨
츰
츱
츳
층
치
칙
친
칟
칠
칡
침
칩
칫
칭
카
칵
칸
칼
캄
캅
캇
캉
캐
캑
캔
캘
캠
캡
캣
캤
캥
캬
캭
컁
커
컥
컨
컫
컬
컴
컵
컷
컸
컹
케
켁
켄
켈
켐
켑
켓
켕
켜
켠
켤
켬
켭
켯
켰
켱
켸
코
콕
콘
콜
콤
콥
콧
콩
콰
콱
콴
콸
쾀
쾅
쾌
쾡
쾨
쾰
쿄
쿠
쿡
쿤
쿨
쿰
쿱
쿳
쿵
쿼
퀀
퀄
퀑
퀘
퀭
퀴
퀵
퀸
퀼
큄
큅
큇
큉
큐
큔
큘
큠
크
큭
큰
클
큼
큽
킁
키
킥
킨
킬
킴
킵
킷
킹
타
탁
탄
탈
탉
탐
탑
탓
탔
탕
태
택
탠
탤
탬
탭
탯
탰
탱
탸
턍
터
턱
턴
털
턺
텀
텁
텃
텄
텅
테
텍
텐
텔
템
텝
텟
텡
텨
텬
텼
톄
톈
토
톡
톤
톨
톰
톱
톳
통
톺
톼
퇀
퇘
퇴
퇸
툇
툉
툐
투
툭
툰
툴
툼
툽
툿
퉁
퉈
퉜
퉤
튀
튁
튄
튈
튐
튑
튕
튜
튠
튤
튬
튱
트
특
튼
튿
틀
틂
틈
틉
틋
틔
틘
틜
틤
틥
티
틱
틴
틸
팀
팁
팃
팅
파
팍
팎
판
팔
팖
팜
팝
팟
팠
팡
팥
패
팩
팬
팰
팸
팹
팻
팼
팽
퍄
퍅
퍼
퍽
펀
펄
펌
펍
펏
펐
펑
페
펙
펜
펠
펨
펩
펫
펭
펴
편
펼
폄
폅
폈
평
폐
폘
폡
폣
포
폭
폰
폴
폼
폽
폿
퐁
퐈
퐝
푀
푄
표
푠
푤
푭
푯
푸
푹
푼
푿
풀
풂
품
풉
풋
풍
풔
풩
퓌
퓐
퓔
퓜
퓟
퓨
퓬
퓰
퓸
퓻
퓽
프
픈
플
픔
픕
픗
피
픽
핀
필
핌
핍
핏
핑
하
학
한
할
핥
함
합
핫
항
해
핵
핸
핼
햄
햅
햇
했
행
햐
향
허
헉
헌
헐
헒
험
헙
헛
헝
헤
헥
헨
헬
헴
헵
헷
헹
혀
혁
현
혈
혐
협
혓
혔
형
혜
혠
혤
혭
호
혹
혼
홀
홅
홈
홉
홋
홍
홑
화
확
환
활
홧
황
홰
홱
홴
횃
횅
회
획
횐
횔
횝
횟
횡
효
횬
횰
횹
횻
후
훅
훈
훌
훑
훔
훗
훙
훠
훤
훨
훰
훵
훼
훽
휀
휄
휑
휘
휙
휜
휠
휨
휩
휫
휭
휴
휵
휸
휼
흄
흇
흉
흐
흑
흔
흖
흗
흘
흙
흠
흡
흣
흥
흩
희
흰
흴
흼
흽
힁
히
힉
힌
힐
힘
힙
힛
힝
다
하
지
이
기
리
가
사
자
대
적
어
아
시
장
수
되
전
상
소
부
정
나
인
일
그
주
고
도
히
구
비
치
보
제
스
오
무
생
마
신
서
연
로
내
성
학
실
화
중
공
한
국
해
관
우
여
식
문
미
용
원
의
교
방
바
간
거
음
발
모
경
조
위
저
만
개
세
요
반
물
안
르
차
외
심
분
단
통
유
선
속
계
예
과
불
금
달
입
점
동
감
출
행
산
래
진
양
회
명
재
당
려
초
체
말
러
영
건
강
라
설
집
추
작
남
각
니
피
편
매
근
터
업
버
석
들
절
결
약
직
날
손
배
복
호
표
력
품
없
색
트
활
울
새
머
살
종
청
현
운
타
판
월
면
럽
름
참
형
확
망
야
쪽
임
포
민
역
목
순
별
술
급
올
두
평
년
번
질
데
담
너
늘
천
드
극
후
파
격
증
디
필
혼
습
노
최
창
본
접
깨
길
프
법
루
눈
환
은
잠
앞
십
코
밤
침
난
워
꾸
책
열
독
철
쓰
군
락
잡
벌
움
처
합
씨
토
향
삼
변
능
답
육
키
님
특
먹
갈
송
잘
녀
험
료
태
다
하
지
이
기
리
가
사
자
대
적
어
아
시
장
수
되
전
상
소
부
정
나
인
일
그
주
고
도
히
구
비
치
보
제
스
오
무
생
마
신
서
연
로
내
성
학
실
화
중
공
한
국
해
관
우
여
식
문
미
용
원
의
교
방
바
간
거
음
발
모
경
조
위
저
만
개
세
요
반
물
안
르
차
외
심
분
단
통
유
선
속
계
예
과
불
금
달
입
점
동
감
출
행
산
래
진
양
회
명
재
당
려
초
체
말
러
영
건
강
라
설
집
추
작
남
각
니
피
편
매
근
터
업
버
석
들
절
결
약
직
날
손
배
복
호
표
력
품
없
색
트
활
울
새
머
살
종
청
현
운
타
판
월
면
럽
름
참
형
확
망
야
쪽
임
포
민
역
목
순
별
술
급
올
두
평
년
번
질
데
담
너
늘
천
드
극
후
파
격
증
디
필
혼
습
노
최
창
본
접
깨
길
프
법
루
눈
환
은
잠
앞
십
코
밤
침
난
워
꾸
책
열
독
철
쓰
군
락
잡
벌
움
처
합
씨
토
향
삼
변
능
답
육
키
님
특
먹
갈
송
잘
녀
험
료
태
롭
농
까
더
등
람
백
귀
줄
알
게
권
숙
런
충
애
승
준
욕
함
취
탁
온
못
채
끼
박
밥
림
짜
막
골
얼
투
레
론
항
카
걸
겨
잔
완
언
허
축
립
크
렇
느
논
랑
놓
넘
병
찌
빠
존
몸
밀
곳
튼
른
익
념
맛
족
웃
큰
악
죽
힘
끝
글
련
메
친
광
맞
희
김
갑
째
빨
견
응
싸
풍
록
흔
것
찰
억
네
검
짝
누
흘
녹
팔
으
류
낮
찬
끄
칠
곧
빛
북
휴
탕
득
규
붙
긴
례
슬
찾
놀
린
착
범
효
틀
티
왕
때
졸
있
짓
할
닥
숨
택
염
퇴
좋
척
즈
퍼
층
깔
량
높
섭
짐
뜨
봉
괴
테
늦
묻
궁
져
풀
받
덕
액
겁
객
령
에
쓸
징
갖
총
옆
촌
끊
흐
란
페
밝
섯
몇
엉
쉬
앉
흥
커
널
을
깊
즐
웨
같
얘
돌
볼
굳
끌
튀
몰
께
패
율
넷
꽃
엄
베
첫
쁘
빼
꼭
옷
꺼
많
빗
랗
따
곡
넓
홍
걱
혀
쟁
와
죄
걷
찍
냉
킬
팩
쩌
껏
맡
폭
닷
잊
쌍
씩
녁
팬
딸
곤
좌
닭
컵
옥
멍
빌
쉽
멀
싫
듯
잎
뉴
멋
끗
왼
릇
센
쇠
암
벽
싱
램
</details>
(사용된 한글 데이터)

### 2-2 TFRecord로의 변환
TensorFlow의 표준 입력 형식은 TFRecords로, 원시 이미지 데이터와 해당 라벨을 한 곳에 저장하는 바이너리 형식이다. TensorFlow 모델에 데이터를 더 잘 공급하기 위해 우선적으로 이미지에서 여러 종류의 TFRecords 파일을 생성하였다.
### 2-3 모델 학습하기
데이터의 양이 기존의 3000여 개에서 총 한글의 양에 필적할 정도로 많아졌기 때문에, 
<details>
<summary>접기/펼치기</summary> 
<pre>#!/usr/bin/env python

import argparse
import io
import os

import tensorflow as tf
from tensorflow.python.tools import freeze_graph
from tensorflow.python.tools import optimize_for_inference_lib


SCRIPT_PATH = os.path.dirname(os.path.abspath(__file__))

DEFAULT_LABEL_FILE = os.path.join(SCRIPT_PATH,
                                  './labels/2350-common-hangul.txt')
DEFAULT_TFRECORDS_DIR = os.path.join(SCRIPT_PATH, 'tfrecords-output')
DEFAULT_OUTPUT_DIR = os.path.join(SCRIPT_PATH, 'saved-model')

MODEL_NAME = 'hangul_tensorflow'
IMAGE_WIDTH = 64
IMAGE_HEIGHT = 64

DEFAULT_NUM_EPOCHS = 15
BATCH_SIZE = 100

num_classes = 2350


def _parse_function(example):
    features = tf.parse_single_example(
        example,
        features={
            'image/class/label': tf.FixedLenFeature([], tf.int64),
            'image/encoded': tf.FixedLenFeature([], dtype=tf.string,
                                                default_value='')
        })
    label = features['image/class/label']
    image_encoded = features['image/encoded']

    # Decode the JPEG.
    image = tf.image.decode_jpeg(image_encoded, channels=1)
    image = tf.image.convert_image_dtype(image, dtype=tf.float32)
    image = tf.reshape(image, [IMAGE_WIDTH*IMAGE_HEIGHT])

    # Represent the label as a one hot vector.
    label = tf.stack(tf.one_hot(label, num_classes))
    return image, label


def export_model(model_output_dir, input_node_names, output_node_name):
    """Export the model so we can use it later.

    This will create two Protocol Buffer files in the model output directory.
    These files represent a serialized version of our model with all the
    learned weights and biases. One of the ProtoBuf files is a version
    optimized for inference-only usage.
    """

    name_base = os.path.join(model_output_dir, MODEL_NAME)
    frozen_graph_file = os.path.join(model_output_dir,
                                     'frozen_' + MODEL_NAME + '.pb')
    freeze_graph.freeze_graph(
        name_base + '.pbtxt', None, False, name_base + '.chkp',
        output_node_name, "save/restore_all", "save/Const:0",
        frozen_graph_file, True, ""
    )

    input_graph_def = tf.GraphDef()
    with tf.gfile.Open(frozen_graph_file, "rb") as f:
        input_graph_def.ParseFromString(f.read())

    output_graph_def = optimize_for_inference_lib.optimize_for_inference(
            input_graph_def, input_node_names, [output_node_name],
            tf.float32.as_datatype_enum)

    optimized_graph_file = os.path.join(model_output_dir,
                                        'optimized_' + MODEL_NAME + '.pb')
    with tf.gfile.GFile(optimized_graph_file, "wb") as f:
        f.write(output_graph_def.SerializeToString())

    print("Inference optimized graph saved at: " + optimized_graph_file)


def weight_variable(shape):
    """Generates a weight variable of a given shape."""
    initial = tf.random.truncated_normal(shape, stddev=0.1)
    return tf.Variable(initial, name='weight')


def bias_variable(shape):
    """Generates a bias variable of a given shape."""
    initial = tf.constant(0.1, shape=shape)
    return tf.Variable(initial, name='bias')


def main(label_file, tfrecords_dir, model_output_dir, num_train_epochs):
    """Perform graph definition and model training.

    Here we will first create our input pipeline for reading in TFRecords
    files and producing random batches of images and labels.
    Next, a convolutional neural network is defined, and training is performed.
    After training, the model is exported to be used in applications.
    """
    global num_classes
    labels = io.open(label_file, 'r', encoding='utf-8').read().splitlines()
    num_classes = len(labels)

    # Define names so we can later reference specific nodes for when we use
    # the model for inference later.
    input_node_name = 'input'
    keep_prob_node_name = 'keep_prob'
    output_node_name = 'output'

    if not os.path.exists(model_output_dir):
        os.makedirs(model_output_dir)

    print('Processing data...')

    tf_record_pattern = os.path.join(tfrecords_dir, '%s-*' % 'train')
    train_data_files = tf.gfile.Glob(tf_record_pattern)

    tf_record_pattern = os.path.join(tfrecords_dir, '%s-*' % 'test')
    test_data_files = tf.gfile.Glob(tf_record_pattern)

    # Create training dataset input pipeline.
    train_dataset = tf.data.TFRecordDataset(train_data_files) \
        .map(_parse_function) \
        .shuffle(1000) \
        .repeat(num_train_epochs) \
        .batch(BATCH_SIZE) \
        .prefetch(1)

    # Create the model!

    # Placeholder to feed in image data.
    x = tf.placeholder(tf.float32, [None, IMAGE_WIDTH*IMAGE_HEIGHT],
                       name=input_node_name)
    # Placeholder to feed in label data. Labels are represented as one_hot
    # vectors.
    y_ = tf.placeholder(tf.float32, [None, num_classes])

    # Reshape the image back into two dimensions so we can perform convolution.
    x_image = tf.reshape(x, [-1, IMAGE_WIDTH, IMAGE_HEIGHT, 1])

    # First convolutional layer. 32 feature maps.
    W_conv1 = weight_variable([5, 5, 1, 32])
    b_conv1 = bias_variable([32])
    x_conv1 = tf.nn.conv2d(x_image, W_conv1, strides=[1, 1, 1, 1],
                           padding='SAME')
    h_conv1 = tf.nn.relu(x_conv1 + b_conv1)

    # Max-pooling.
    h_pool1 = tf.nn.max_pool(h_conv1, ksize=[1, 2, 2, 1],
                             strides=[1, 2, 2, 1], padding='SAME')

    # Second convolutional layer. 64 feature maps.
    W_conv2 = weight_variable([5, 5, 32, 64])
    b_conv2 = bias_variable([64])
    x_conv2 = tf.nn.conv2d(h_pool1, W_conv2, strides=[1, 1, 1, 1],
                           padding='SAME')
    h_conv2 = tf.nn.relu(x_conv2 + b_conv2)

    h_pool2 = tf.nn.max_pool(h_conv2, ksize=[1, 2, 2, 1],
                             strides=[1, 2, 2, 1], padding='SAME')

    # Third convolutional layer. 128 feature maps.
    W_conv3 = weight_variable([3, 3, 64, 128])
    b_conv3 = bias_variable([128])
    x_conv3 = tf.nn.conv2d(h_pool2, W_conv3, strides=[1, 1, 1, 1],
                           padding='SAME')
    h_conv3 = tf.nn.relu(x_conv3 + b_conv3)

    h_pool3 = tf.nn.max_pool(h_conv3, ksize=[1, 2, 2, 1],
                             strides=[1, 2, 2, 1], padding='SAME')

    # Fully connected layer. Here we choose to have 1024 neurons in this layer.
    h_pool_flat = tf.reshape(h_pool3, [-1, 8*8*128])
    W_fc1 = weight_variable([8*8*128, 1024])
    b_fc1 = bias_variable([1024])
    h_fc1 = tf.nn.relu(tf.matmul(h_pool_flat, W_fc1) + b_fc1)

    # Dropout layer. This helps fight overfitting.
    keep_prob = tf.placeholder(tf.float32, name=keep_prob_node_name)
    h_fc1_drop = tf.nn.dropout(h_fc1, rate=1-keep_prob)

    # Classification layer.
    W_fc2 = weight_variable([1024, num_classes])
    b_fc2 = bias_variable([num_classes])
    y = tf.matmul(h_fc1_drop, W_fc2) + b_fc2

    # This isn't used for training, but for when using the saved model.
    tf.nn.softmax(y, name=output_node_name)

    # Define our loss.
    cross_entropy = tf.reduce_mean(
        tf.nn.softmax_cross_entropy_with_logits_v2(
            labels=tf.stop_gradient(y_),
            logits=y
        )
    )

    # Define our optimizer for minimizing our loss. Here we choose a learning
    # rate of 0.0001 with AdamOptimizer. This utilizes someting
    # called the Adam algorithm, and utilizes adaptive learning rates and
    # momentum to get past saddle points.
    train_step = tf.train.AdamOptimizer(0.0001).minimize(cross_entropy)

    # Define accuracy.
    correct_prediction = tf.equal(tf.argmax(y, 1), tf.argmax(y_, 1))
    correct_prediction = tf.cast(correct_prediction, tf.float32)
    accuracy = tf.reduce_mean(correct_prediction)

    saver = tf.train.Saver()

    with tf.Session() as sess:
        # Initialize the variables.
        sess.run(tf.global_variables_initializer())

        checkpoint_file = os.path.join(model_output_dir, MODEL_NAME + '.chkp')

        # Save the graph definition to a file.
        tf.train.write_graph(sess.graph_def, model_output_dir,
                             MODEL_NAME + '.pbtxt', True)

        try:
            iterator = train_dataset.make_one_shot_iterator()
            batch = iterator.get_next()
            step = 0

            while True:

                # Get a batch of images and their corresponding labels.
                train_images, train_labels = sess.run(batch)

                # Perform the training step, feeding in the batches.
                sess.run(train_step, feed_dict={x: train_images,
                                                y_: train_labels,
                                                keep_prob: 0.5})
                if step % 100 == 0:
                    train_accuracy = sess.run(
                        accuracy,
                        feed_dict={x: train_images, y_: train_labels,
                                   keep_prob: 1.0}
                    )
                    print("Step %d, Training Accuracy %g" %
                          (step, float(train_accuracy)))

                # Every 10,000 iterations, we save a checkpoint of the model.
                if step % 10000 == 0:
                    saver.save(sess, checkpoint_file, global_step=step)

                step += 1

        except tf.errors.OutOfRangeError:
            pass

        # Save a checkpoint after training has completed.
        saver.save(sess, checkpoint_file)

        # See how model did by running the testing set through the model.
        print('Testing model...')

        # Create testing dataset input pipeline.
        test_dataset = tf.data.TFRecordDataset(test_data_files) \
            .map(_parse_function) \
            .batch(BATCH_SIZE) \
            .prefetch(1)

        # Define a different tensor operation for summing the correct
        # predictions.
        accuracy2 = tf.reduce_sum(correct_prediction)
        total_correct_preds = 0
        total_preds = 0

        try:
            iterator = test_dataset.make_one_shot_iterator()
            batch = iterator.get_next()
            while True:
                test_images, test_labels = sess.run(batch)
                acc = sess.run(accuracy2, feed_dict={x: test_images,
                                                     y_: test_labels,
                                                     keep_prob: 1.0})
                total_preds += len(test_images)
                total_correct_preds += acc

        except tf.errors.OutOfRangeError:
            pass

        test_accuracy = total_correct_preds/total_preds
        print("Testing Accuracy {}".format(test_accuracy))

        export_model(model_output_dir, [input_node_name, keep_prob_node_name],
                     output_node_name)

        sess.close()


if __name__ == '__main__':
    parser = argparse.ArgumentParser()
    parser.add_argument('--label-file', type=str, dest='label_file',
                        default=DEFAULT_LABEL_FILE,
                        help='File containing newline delimited labels.')
    parser.add_argument('--tfrecords-dir', type=str, dest='tfrecords_dir',
                        default=DEFAULT_TFRECORDS_DIR,
                        help='Directory of TFRecords files.')
    parser.add_argument('--output-dir', type=str, dest='output_dir',
                        default=DEFAULT_OUTPUT_DIR,
                        help='Output directory to store saved model files.')
    parser.add_argument('--num-train-epochs', type=int,
                        dest='num_train_epochs',
                        default=DEFAULT_NUM_EPOCHS,
                        help='Number of times to iterate over all of the '
                             'training data.')
    args = parser.parse_args()
    main(args.label_file, args.tfrecords_dir,
         args.output_dir, args.num_train_epochs)
         </pre>
         </details>
(데이터 양을 늘리기 위해 사용한 스크립트)
해당 스크립트는 입력 파이프라인을 생성하고, 이미지와 라벨의 랜덤 배치 및 생성을 처리하며, CNN을 정의하며 훈련을 진행한다. 훈련 한 이후에는 안드로이드 애플리케이션에서 사용 가능하게 모델을 내보낸다.
### 2-4 텍스트 인식의 순서
먼저 온라인에서 한글 지원 폰트를 가져와 이미지 데이터를 생성하고, 탄성 변환을 진행한 후, MNIST 형식으로 변환한다. 그 후 이미지를 TFRecord 형식으로 변환하여 입력 데이터로 사용하고, 모델을 훈련한다. 마지막으로 모델을 안드로이드 애플리케이션에 저장한다.
## 3. 딥러닝과 OCR
### 3-1 딥러닝 모델과 OCR
딥러닝은 여러 종류의 OCR 작업 모델을 학습시키는데, CNN과 RNN 구조가 포함된다.
* CNN 구조: 합성곱 신경망으로, 주로 이미지 및 동영상과 같은 그래픽 데이터의 처리에 사용된다. 합성곱 계층(Convolutional layer)을 사용하여 지역적 패턴 및 특징을 추출하고, 최대 풀링 레이어(Max pooling layer)를 통해 공간 차원을 축소시키며, 지역적 특징을 강화한다. 이후 여러 합성곱 및 풀링 레이어를 쌓아 복잡한 특징을 추출하고, 완전 연결 레이어(Fully connected layer)를 통해 분류나 회귀 문제를 해결한다. 특히, 알고리즘 설계자가 영상이나 이미지의 특성을 미리 파악하여 수제작된 필터를 거치는 과정을 제거하여 이미지 인식, 물체 감지, 얼굴 인식, 패턴 인식과 같은 일에 효율적이다.
* RNN 구조: 순차 데이터나 시계열 데이터와 같은 순서가 있는 시퀀스 데이터를 처리하는 데 사용된다. 순환 계층(Recurrent layer)을 사용하여 현재 입력과 이전 상태를 함께 고려하여 순차 정보를 처리한다. 또한, 입력된 시퀀스의 길이와는 상관없이 처리할 수 있어 다양한 길이의 입력을 다룰 수 있으며, 셀, 입력 게이트, 출력 게이트, 망각 게이트를 이용하는 LTSM과 같은 구조를 이용하기도 한다. 순차적인 데이터들의 처리에 유리하여 자연어 처리, 음성 인식 등과 같은 문제에 효율적이다.
<br> CNN은 우선 이미지에서 특징을 추출하는 역할을 하고, 그 후 RNN 모델이 시퀀스 데이터(텍스트 라인)를 처리하여 효율적인 텍스트 인식을 구현할 수 있다.

### 3-2 학습 데이터
OCR 모델의 학습을 위해서는 방대한 양의 학습 데이터가 필요하다. 이 데이터에는 다양한 폰트, 글자 크기, 필체, 손글씨 등이 포함되어야 딥 러닝 모델이 이러한 다양한 데이터를 학습하여 비교적 더 다양하고 불리한 조건에서도 정확하게 텍스트를 인식할 수 있게 된다. 또한, 기계 학습을 통해 글자의 틀을 벗어나지 않으면서도 변형된 글씨를 만들어 낼 수 있어 학습 데이터의 생성에 있어서도 유용한 점이 존재한다.

### 3-3 OCR 성능의 향상
딥러닝은 OCR 기술의 정확성 및 성능을 향상시킬 수 있다. 모델의 최적화, 데이터 전처리, 모델 구조 설계 등을 딥러닝을 통해 구현하여 OCR의 성능을 지속적으로 개선시킬 수 있다.

## 4. 실험 과정 중 한계
### 4-1 GPU 성능의 한계
실험한 PC의 GPU 성능의 한계로 인해 데이터 학습에 어려움이 있었다. 또한, 학습시킨 데이터의 양이 적어 텍스트 인식의 정확성이 전체 데이터를 이용하였을 경우에 비해 현저히 떨어졌다.
### 4-2 지식의 한계
UI/UX 디자인에 대한 지식이 부족하여, 사용자가 사용하기 어렵고, 상호작용이 매끄럽지 못한 UI를 가진 안드로이드 애플리케이션이 만들어졌다.
### 4-3 GPU 성능에 대한 대안
모든 데이터를 생성하는 대신, 일부 데이터를 생성한 후, 그 데이터를 사용하여 학습한 결과를 이용하였다. 그럼에도 불구하고, GPU 성능에 제약을 받아 완전한 인공 신경망을 구축하지는 못하였고, 추후 더 높은 성능의 GPU로 작업할 예정이다.
### 4-4 UI에 대한 대안
UX/UI 디자인에 대한 연구를 하여, 추후에 보완하고자 하였다.
### 4-5 한글의 특성으로 인한 연구의 어려움
현대 한글의 모든 글자인 11172자는 물론, 사용 빈도가 그나마 있다고 추정되는 KS X 1001 완성형에 포함된 2350자의 한글만 해도 인식하는 데에 어려움이 존재한다.
## 5. 발전 가능성에 대한 고찰
### 5-1 문맥에 대한 고려
기존의 OCR과는 다르게, 텍스트의 문맥 또한 고려한다면 비록 텍스트 자체를 인식하는 데에 실패하였더라도, 문맥을 통해 가장 적합한 글자를 부여할 수 있을 것이다.
### 5-2 실제로 사용되는 글자에 대한 고려
싻, 쏇, 쀏 등과 같이 실생활에서 거의 사용되지 않는 글자 역시도 학습 대상에 포함되어 있어 오히려 인식의 정확도 및 모델의 성능만을 낮추고 있는 상황을 만들어내고 있다. 한글에 대한 추가적인 연구를 통해 빅데이터를 구축하여 그것을 기반으로 실질적으로 사용되는 글자만을 선별적으로 학습시키는 방안을 선택해야 할 것이다.
## 6. 출처 및 참고 문헌
* OCR한글폰트의 설계에 관한 연구 - 한국통신학회 1988년도 추계학술발표회 논문집 1988 Oct. 01, 1988년, pp.251 - 256  
김재성 (인하대학교 전자계산학과);  김홍윤 (인하대학교 전자계산학과);  김홍일 (인하대학교 전자계산학과);  이균하 (인하대학교 전자계산학과)
* 딥러닝을 활용한 한글문장 OCR연구 - 한국정보과학회언어공학연구회 2019년도 제31회 한글 및 한국어 정보처리 학술대회 2019 Oct. 10, 2019년, pp.470 - 474  
박선우 (모두의연구소)
* 딥러닝을 위한 인공신경망 - 오창석
* KAIST 김진형 교수에게 듣는 AI 최강의 수업 - 김진형
* Naver Clova-What Is Wrong With Scene Text Recognition Model Comparisons?
Dataset and Model Analysis-Jeonghun Baek, Geewook Kim, Junyeop Lee, Sungrae Park, Dongyoon Han, Sangdoo Yun, Seong Joon Oh, Hwalsuk Lee
* IBM-tensorflow-hangul-recognition
* NHN FORWARD 22-딥러닝 OCR(문자인식) 모델 성능 향상 경험기 - 김연규
