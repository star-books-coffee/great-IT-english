### 1. Git으로 세련되게 협업하는 5가지 방법

- 전 세계적으로 통용되는 커밋 메시지 관습 : Conventional Commits
- 커밋 메시지는 Subject (Title), Body, Footer로 구분됨
- Conventional Commits의 구조
    > <type[optional scope]:<description> <br>
    [optional body] <br>
    [optional footer(s)]
    > 
    - docs(readme): update build instructions ［문서(readme) 빌드 지침 업데이트］
    
    → 선택적으로 (readme) 와 같이 **변경 내역이 적용되는 범위와 맥락을 표시**
    
- 커밋 메시지에 Conventional Commits를 적용하지 않는 경우, 일반적으로 앞부분만 대문자를 사용하고 type을 생략
- 영문 커밋 메시지 작성법
    1. 명령적 어조의 `동사 원형` 으로 시작하라
        - Fix : 수정하다
        - Bump : 버전을 올리다
        - Wrap : 감싸다, 그룹화하다
    2. 모두 소문자로 또는 첫 글자만 대문자로
    3. 관사 최소화
    4. 마침표(.)와 같은 구두점(Punctuation Mark) 생략
    5. 변경한 이유, 상세 설명은 본문（Body）에
- 주요 실무 영어
    - Squash the last 3 commits ; 최근 3개의 커밋을 합치다
 
### 2. 외국인이 들어도 감탄할 코드 설명법

- `Declare` a (variable / function / class): (변수 / 함수 / 클래스)를 선언하다
- `Assign` a value to a variable : 변수에 값을 할당하다
    - 변수에 초기값 할당 (Assign) 하는 초기하는 `Initialize`
- `Name` a class : 클래스의 이름을 짓다
- `Pass` an argument to a function : 함수에 인자를 전달하다
- `Call` a function : 함수를 호출하다
    - 다른 대상이 함수를 "불러오는" 경우에는 invoke를, 직접 함수를 "호줄하는" 경우에는 call을 사용합니다
    - **함수를 "불러오는" 경우 (Invoke)**
        - **Event Handler**: 웹 페이지에서 버튼을 클릭하면 이벤트 핸들러가 함수를 "불러옵니다"
            
            ```jsx
            button.addEventListener('click', myFunction); // 이벤트 핸들러가 myFunction을 "불러옴" (invoke).
            ```
            
        - **Promise**: 프로미스를 사용하여 비동기 작업을 수행할 때, **`.then()`**을 통해 성공 또는 실패 콜백 함수를 "불러옵니다"
            
            ```jsx
            javascriptCopy code
            fetchData()
              .then(successCallback) // 성공 시 successCallback 함수를 "불러옴" (invoke).
              .catch(errorCallback); // 실패 시 errorCallback 함수를 "불러옴" (invoke).
            
            ```
            
    - **함수를 "호출하는" 경우 (Call)**
        - **직접 함수 호출**: 함수를 직접 호출할 때, 함수를 "호출" (call)
            
            ```jsx
            function add(a, b) {
              return a + b;
            }
            
            const result = add(3, 5); // 함수 add를 "호출" (call) 함.
            ```
       
        - **재귀 함수 호출**: 함수 내에서 자신을 호출할 때, 자기 자신을 "호출"


            ```jsx
            function factorial(n) {
              if (n <= 1) {
                return 1;
              }
              return n * factorial(n - 1); // 자신을 "호출" (call) 함.
            }
            
            const result = factorial(5);
            ```
- `Execute (Run)` a loop body : 반복문의 내용을 수행하다
- `Iterate over` (through) an array : 배열을 돌면서 반복하다
- The conditional statement `evaluates to true` : 조건문이 참으로 평가되다
- `Jump out of` a loop : 반복문에서 빠져나오다
    - break
- `Jump over` an iteration : 반복을 한 번 건너뛰다
    - continue
- `Increment / Decrement` the variable `by 2` : 변수를 2만큼 증가시키다 / 감소시키다
More
    - Increment the variable i in the for loop by 1 : for 반복문의 i를 1 만큼 증가시키다

### 3. 인생은 실전, 개발 현장 속에서 배우는 실전 영어

- Hug is the fastest growing framework for microservices on Python3 and `as such` clearly `deserves placement on` this list.
    - As such : "그러한 이유로, 그 자체로(in itself)”
    - 그 자체로 리스트에 배치(placement)될 자격이 있다(deserve)
- **(I’m)** `Not sure` if this is the right place but I would go for a Services or Microservices section.
    - 캐주얼한 커뮤니케이션에서는 주어 및 형용사와 함께 사용되는 be 동사가 종종 생략됨
- This is where I'd ideally want to place it, and `as time goes on` I believe there will be more and more libraries that would `aptly` fit in this category.
    - As time goes on (by) : 시간이 지남에 따라
    - aptly : 적절하게 (properly)
        - aptly fit : 적절하게 맞는
- `With all due respect`, do some basic research before making such `blatantly` false statements.
    - With all due respect : 외람되지만, 이런 말씀드려서 죄송하지만
    - blantantly : 노골적으로, 직설적으로
- It allows your APIs to be `exposed` over the command line as well as over HTTP
    - Expose : 드러내다, 노출되다와 같이 사용되지만 IT 업계에서는 무언가를 공개해서 사용 가능하게 하다(make available) 라는 의미로 사용
- Workflow jobs run on self-hosted runners `on` AWS Graviton instances
    - on : AWS, Azure, GCP와 같은 **클라우드에 업로드된 인스턴스(Instance, 가상 서버)** 앞에서 사용
- PR `on` master branch
    - Pull request와 Commit은 Branch 위에 (on) 있다고 표현
    - 반면, Branch는 Repository 안에(in) 있다고 표현
        - How many branches do we have `in` this repository?
- `Nightly` on master branch at 8am UTC
    - Nightly build : 일일 빌드(주기적인 테스트를 위해 매일 생성하는 빌드)
- `Revision` : 수정, 개정
- What led you to use these files for the tests (our [CONTRIBUTING.md](http://CONTRIBUTING.md) perhaps)?
    - 무엇이 너가 이 파일들을 사용하도록 이끌었니? == 어떻게 이 파일들을 사용하게 되었니?
- Can we work next on upgrading to a different setup, after we get it working in its current `iteration`?
    - iteration : 개발 사이클 1번 (a single development cycle), 반복
- We were planning to deprecate the rest, especially pip_new.sh which is `inscrutable`
    - inscrutable : 이해하기 어려운
- `LGTM` : "Looks Good To Me"의 약어로, 문제 없어 보인다라는 뜻
- `Explanatory` : 설명하는, 설명적인
- I think the `intent` to clarify here is good but I'd maybe add the logic to line 243 **and not what is essentially a custom toString for error messages in this file.**
    - 여기에서 이를 명확히 하려는 **`의도`**가 좋다고 생각하지만, 저라면 본질적으로 **커스텀 toString을 위한 이 파일의 오류 메시지가 아닌, 243** 라인에 로직을 추가할 것 같습니다.
- prominent : 눈에 띄는, 두드러진
- You might be `missing out on` errors
    - Miss out on : (기회나 상황을) 놓치다
- However, lots of other errors that throw in React are designed to be `preceded` by a console. error
    - precede : ~에 앞서다, 선행하다
- You would be shown a `misleading` late error
    - misleading : "오해의 소지가 있는

### 4. 오픈소스 커뮤니티 “인싸” 로 도약하는 인터넷 영어 표현

- `LGTM (looks good to me)` : PR 코드 리뷰에서 별다른 문제가 없을 때 사용
- `TL；DR (Too Long; Didn't Read)` : 너무 길어서 읽지 않는다라는 뜻으로, 주로 기술 블로그나 문서에서 자세한 설명을 시작하기 전에 요약된 정보를 소개할 때 사용
- `SSIA (Subject Says It All)` : "제목이 모든 것을 말한다” (ㅈㄱㄴ),  제목 외에 별도의 설명이 필요 없는 경우
- `TBD (To Be Determined)` : 아직 결정되지 않은 내용이 있어, 나중에 결정해야 함을 의미
- `RFC (Request For Comments)` : 풀 리퀘스트와 같이 새로운 것을 제안하거나 포럼에서 무언가를 제안할 때, 의견을 요청하기 위해 사용
- `In My Honest Opinion` : "제 솔직한 생각으로"
- `In My Humble Opinion` : 겸손한 느낌을 담은 " 제 소견으로는"
- `AFAIK (As Far As I Know)` : "내가 아는 한", 절대적으로 확실하지는 않지만 알고 있는 정보를 말할 때 사용
- `FYI (For Your Information)` : ''참고로"라는 의미로 다른 사람과 정보를 공유할 때 사용
ex) FYI, this API is deprecated. / 참고로, 이 API는 더 이상 권장되지 않습니다.
- `TIA (Thanks In Advance)` : "미리 감사합니다"라는 뜻으로 다른 사람에게 도움을 요청할 때 사용
- `AFK (Away From Keyboard)` : "키보드에서 떨어진"이라는 뜻으로 자리를 비우거나 휴가 중일 때 사용
    - 휴가 중인 경우는 OOO(Out Of Office)라는 약어도 자주 사용
- `Noob` : "입문자 (Newbie)", 새로 참여하는 오픈소스 커뮤니티 또는 프로젝트에 자신을 소개할 때 사용
- `WIP (Work In Progress)` : 진행 중, 진행 중인 작업

### 5. 퇴근 시간을 앞당기는 검색 노하우 4가지

1. 핵심 키워드를 “ “ 로 묶기
    - "Express, Django"을 **키워드로 반드시 포함**하려면 Whk:h is the best backend framework among "Express", "Django" 과 같이 따음표로 핵심 키워드를 감싸주면 됨
    - "Express, Django, and Laraval"과 같이 **여러 단어를 그룹화하여 쌍따옴표로 묶을 경우** "Express, Django, and Laravel" **그룹 키워드와 정확하게 일치하는** 자료를 찾을 수 있음
        - 즉, "Laravel, Express, and Django"라는 콘텐츠를 포함한 웹페이지는 검색되지 않음
2. 특정 웹사이트에서만 검색 결과 가져오기
    - 특정 웹페이지의 검색 결과만을 확인하려면 검색어에 "**site:도메인**" 키워드 추가
        - 스택오버플로우에서 C++의 메모리 유출 문제 해결 방법을 검색하려면
        "how to fix memory leaks in C++ `site：[stackoverflow.com](http://stackoverflow.com/)`"와 같이 검색
    - 검색어 뒤에 "**filetype：확장자**"를 추가하면 해당 확장자의 파일 검색 가능
        - Python Cheat Sheet filetype:pdf 로 검색하면, Python Cheat Sheet PDF 찾을 수 있음
    - 검색 키워드에 ***는 와일드카드**(Wildcard, 다른 단어나 문장으로 대체될 수 있는 부분) 역할
    - 마이너스(-) 연산자는 **특정 단어를 뺀 검색 결과**를, 플러스(+) 연산자는 **특정 단어를 포함한 검색 결과**
3. 중요 단어만 포함해서, 단순하게
    - 기술 문서를 검색할 때도 장황한 문장보다는 핵심 키워드로만으로 검색하는 것이 훨씬 효과적
4. 웹페이지가 사용할만한 키워드로 검색하기
    - 일상적인 표현으로 구성된 키워드보다는 웹페이지가 포함할 만한 단어로 키워드를 구성하기
    - "My iOS app keeps closing"보다는 "Crashing iOS app”

### 6. 단어 하나로 생사가 갈리는 소프트웨어 법률 영어

- 영어 법률 문서의 특징
1. 조동사 Shall, May 의 빈번한 사용
    - `Shall`: 반드시 지켜야 하는 것
    - `May`: 허용되는 것
2. 법률 문서는 시작 부분에 문서에서 다룰 주요 용어를 정의함
    ```
    associated documentation files (the "Software")
    이와 연관된 모든 문서 파일들 (이하 "소프트웨어"라 한다)
    ```
    - `이하 ~라 한다` 라고 정의하는 것처럼, 영어 법률 문서는 (the "Software")와 같이 용어의 첫번째 글자를 대문자로 쓰고, 용어가 처음 정의되는 부분을 큰 따옴표로 표시
3. 강조가 필요한 부분, 법적 책임 소재를 명시하는 부분은 대문자로 표시
4. 문장 사이의 관계나 법률 문서의 성격을 강조하기 위해 hereto(여기에), hereafter(이후로), thereof(앞서 언급된 그것의) 와 같은 대명사형 부사 사용

- MIT 라이선스 예시
    - `free of charge` : 무료로
    - `sublicense` : 특허를 양도하다, 재실시하다, 2차 라이선스를 부여하다
    - `subject to` : ~를 조건으로, 조건에 따라
        - ex) subject to the following conditions) 아래 조건에 따라
        - terms : 서비스 사용 전 합의되어야 하는 조건
        - conditions : 서비스 중에 준수해야 하는 조건
    - substanstial : (양, 가치, 중요성이) 상당한
    - `as is` : (어떤 조건, 상태에서든) 있는 그대로
    - `liable for` : ~에 대한 책임이 있는, ~에 대한 의무가 있는
    - `or otherwise` : (앞서 언급한 것의) 또는 그 반대, (앞서 언급한 것) 이든 그 외 다른 것이든
    - `out of` : ~로부터, ~도중에

- IT 주요 법률 영어
    - Terms and conditions : 이용 약관
    - Copyleft : 공개저작권
    - Patent : 특허권
    - Liability : 법적 책임, 부채
 
### 7. 품격 있게 비즈니스 이메일을 작성하는 방법

1. **제목**
    - Regarding (~에 대하여) 로 시작하기도 함
        - Regarding Technical Support
    - 관사 생략하여 최대한 간소화
    - 상대방 조치 필요한 경우 Action Required, Urgent 붙임
2. **본문**
    
    1) 호칭
    - 수신인이 특정되지 않은 경우 `Whom it may concern (연관될 수 있는 사람)` 이라는 표현 사용
    - Hello 는 Hi 보다 조금 더 격식 갖춘 인사말 (IT 업계는 처음 대화하는 상대방과도 hi 사용하는 경우가 많음)
    
    2) 인사
    - I hope you are doing well.
    - I hope all is well, I hope you are well.
        - 잘 지내고 있기를 바랍니다
    - I hope this email finds you well.
        - 이 이메일이 잘 전달되기를 바랍니다
    - 주말이 끝나거나 휴가에서 복귀하는 경우
        - I hope you enjoyed your weekend. : 즐거운 주말이 되셨기를 바랍니다
        - I hope you had a great vacation. : 멋진 휴가 보내셨기를 바랍니다
    
    3) 본문
    - 영문 이메일은 한국 이메일보다 **간결함을 중요시**하며, 서문 없이 본론으로 바로 들어가는 경우가 많음
        - I’m writing to
        - I’m emailing to
    
    4) 요청
    
    - 정중한 표현이 필요한 경우
        - Could you please ~?
        - I'd like to request
        - I would appreciate it if you could ~
    - 지나치게 격식을 갖출 필요가 없는 상황에서는 Can you ~? / Please ~ 로 요청함
  
3. **마무리**
    
    1) 마무리 인사 : **이메일 본론과 맺음말 사이**에 작성
    
    - `Please feel free to contact me` for more information.
    - I `look forward to your response`. ( I look forward to hearing from you)
    - Thank you for your time.
    - Don’t `hesitate to contact me` for further assistant
    
    2) 맺음말 
    
    - With Kind Regards
    - Best Regards
    - Regards
    - Sincerely
- 나는, 저는과 같이 자신을 직접적으로 드러내는 표현을 자제하는 한국식 이메일과 달리, **영문 이메일은 주어를 포함해서 작성하는 것이 일반적**
<br>

- 리마인더와 관련된 표현
    - `Gentle reminder, Friendly reminder` <br>
    ex) This is a gentle reminder that your document review is due this Friday.
- 감사 표현
    - `Express my (our) gratitude` : 조금 더 격식있는 표현 <br>
    ex) I would like to express my (sincere) gratitude for your support.
- 양해를 구하는 표현
    - `Thank you for your patience` : (앞으로 불편이나 지연이 있을 수 있으니) 양해를 구한다와 같이 **간접적으로 양해 구할 때도 사용**
