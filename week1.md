## 퀘스트 1: 칭찬받기 자료조사

거의 모든 캠퍼 분들이 밤을 새우시면서 매일매일 미션을 진행하시고 계십니다.

이 힘든 과정을 진행하면서 누군가가 내가 잘한점을 항상 칭찬해준다면 어떨까요?

**칭찬은 고래도 춤추게 한다**

이 자료는 좋은 퀄리티의 코드를 리뷰하는 방법을 이야기하지만, 칭찬이 개발자에게 어떤 좋은 영향을 끼치는지 나와있습니다.

출처:

- https://www.slideshare.net/slideshow/improve-quality-and-morale-using-peer-code-reviews/8317067

- https://mende.io/blog/improving-developer-experience-starting-with-psychological-safety-team-stability-and-work-life-balance/?utm_source=chatgpt.com

아직 시장에 전용 “학습정리 칭찬 AI” 서비스는 드물지만,

    - 대형 언어 모델(ChatGPT 등)에 맞춤 프롬프트를 건네거나
    - 기존 글쓰기 보조 툴의 강점 리포트를 활용하거나
    - 직접 간단한 챗봇을 제작하는 방식으로
    - 충분히 “정리한 내용에 대한 구체적 칭찬”을 자동화할 수 있습니다.

입력 예시:

> ChatGPT가 요구하는 프롬프트를 작성했습니다.

```text
아래는 제가 이번 미션마다 작성한 학습정리.md 내용입니다.
문서 구조·내용·표현 관점에서 “잘한 점” 3가지를 구체적으로 짚어 칭찬해 주세요.
각 포인트별로 어떤 부분이 좋았는지, 그리고 그 장점이 학습에 어떻게 도움이 되는지도 함께 설명해 주시면 감사하겠습니다.

―――
[여기에 학습정리.md 내용을 통째로 붙여넣으세요]
―――
```

> 시간이 여유가 있다면 직접 챗봇을 구현하는 것도 좋을 것 같습니다.

### 맞춤형 “칭찬 봇” 구축하기

- Slack, Discord 같은 채팅 플랫폼에서 OpenAI API + 간단한 서버(예: Node.js)만 있으면
  1. 사용자가 파일을 업로드하거나 슬랙에 붙여넣으면
  2. 백엔드가 AI에 “유저 노트 분석 → 칭찬 3가지” 요청
  3. 자동으로 응답해 주는 봇을 만들 수 있습니다.

---

## 퀘스트 2: 기분에 맞는 **이미지** 수집하기

#### 질문 / 고민

처음엔 단순히 **슬랙 프로필 이미지를 AI로 만들어보면** 어떨까 했습니다.<br>
`TEXT-to-IMAGE AI` 툴을 쓰면 내가 원하는 분위기나 정체성을 담은 이미지를 만들 수 있으니까요.

그런데 작업을 하다 보니,  
“**하루하루 기분을 이미지로 남기면 내 프로필도 계속 변하는 게 아닐까?**”  
라는 생각이 들었고, 그게 점점 **기록 습관**과 **감정 표현**이라는 주제로 확장됐습니다.

> 그날의 기분을 이미지로 남긴다면, 더 의미 있는 회고가 가능하지 않을까?

> [NAVER CLOVA 블로그 - 음성으로 소통하는 AI, 사람의 감정까지 이해하다](https://clova.ai/tech-blog/%EC%9D%8C%EC%84%B1%EC%9C%BC%EB%A1%9C-%EC%86%8C%ED%86%B5%ED%95%98%EB%8A%94-ai-%EC%82%AC%EB%9E%8C%EC%9D%98-%EA%B0%90%EC%A0%95%EA%B9%8C%EC%A7%80-%EC%9D%B4%ED%95%B4%ED%95%98%EB%8B%A4)

퀘스트 2의 목적은 단순한 이미지 생성이 아닌,  
**AI를 통해 감정을 표현하고 기록하는 루틴을 만드는 것**입니다.

감정은 단순히 말로만 표현되는 것이 아니라,  
**목소리, 표정, 이미지**와 같은 다양한 표현 매체로 감지되고 표현될 수 있습니다.

<img src="https://clova.ai/cdn/media/2024/11/thumbnail_techblog_HCX_EC9D8CEC84B1EC9CBCEBA19CEC868CED86B5ED9598EB8A94AI_A.png" alt="clova" width=600>

**NAVER CLOVA의 연구**는 이 지점에서 큰 인사이트를 주었습니다.

> *AI가 사람의 음성 속 감정적 특징을 분석해 상황에 따라 반응하는 기술*이 존재한다는 것은,  
> 우리의 기분이 충분히 기술로 감지되고 표현될 수 있다는 가능성을 열어줍니다.

우리는 매일 `README`를 작성합니다.  
어떤 날은 복잡하고, 답답한 심정이 들기도 하겠죠.  
그럴 때 **기분을 이미지로 남기는 활동**은 감정 기록의 새로운 대안이자,  
기술과 연결된 창의적 자기 표현 방식이 될 수 있다고 생각했습니다.

### 오늘의 기분을 AI로 시각화하기

- 매일의 감정을 **키워드**로 정리한다.
- **TEXT-to-IMAGE AI**를 활용해 감정을 시각적으로 표현한다.
- 생성된 이미지를 `README`나 노션 등에 저장해 **루틴처럼 기록**한다.

감정은 텍스트로 직접 정리할 수도 있고,  
CLOVA의 음성 감정 인식처럼,<br>다양한 방식으로 감정이 기술에 의해 포착될 수 있다는 점에서  
우리는 그 감정을 **텍스트 형태로 AI에게 전달하고**,  
**시각적 이미지로 표현하는 루틴**을 만들어 볼 수 있습니다.

즉, 감정 인식 기술은 **AI가 감정을 이해할 수 있다는 가능성**을 보여주고,  
TEXT-to-IMAGE AI는 **그 감정을 시각적으로 표현하는 수단**이 될 수 있습니다.

그렇게 매일의 감정을 이미지로 남기는 활동은 단순한 기록을 넘어,  
**기술을 활용한 감정 루틴**, 그리고 **자기 인식의 새로운 방법**이 될 수 있습니다.

## AI를 통한 README 자동 요약

### 대상 파일 수집

1. Gist API를 통해 gist의 README를 자동으로 가져오도록 구성
2. [README.md](http://README.md)의 RAW를 이용해서 Get 요청을 통해 바로 README.md의 내용을 가져옴

### 요약

1. OpenAI API를 통해 가져온 README의 내용을 요약

### 자동화

1. Python 스크립트로 처리
2. 크론탭 or GitHub Action을 통해 자동 실행
   - Python 스크립트
     - 가져온 README.md의 내용을 OpenAI API를 통해 요약
     - 요약 내용을 바탕으로 Summary.md를 생성
   - Summary를 gist에 push

### 문제 가능성

- secret gist 문제
  - GitHub Actions을 통해 자동화를 진행한다면 별도의 인증이 필요없음

---

## 퀘스트 4: AI에게 배우기, 자료 추천받아서 더 똑똑하게 공부하기

### 배경

요즘 미션을 수행할 때, 단순히 "제출"을 넘어서 진짜 나의 것으로 만들고 싶다는 욕심이 생깁니다.

개념을 더 깊이 파고들고 싶은데,막상 구글링을 하면 </br>
“무엇을 검색해야 할지도 모르겠고”, “정보는 너무 흩어져 있거나 피상적”이라 시간만 날릴 때가 많았습니다.

그러다 문득 이런 생각이 들었습니다. "AI에게 미션을 설명하면, 내가 찾고 싶은 자료들을 더 잘 정리해주지 않을까?"

그래서 생성형 AI를 "진짜 학습 파트너" 처럼 써보는 것이 퀘스트의 목표입니다.

### 활용해 볼 수 있는 도구

#### 1. Perplexity

- 검색 + AI 요약.
- 핵심 정보 요약과 함께 출처도 함께 제공돼서 학습 신뢰도 UP

<img width="400" height="767" alt="스크린샷 2025-07-18 오후 4 35 10" src="https://github.com/user-attachments/assets/64ebac4b-e285-4424-9472-e581eb97d433" />

<img width="400" height="742" alt="스크린샷 2025-07-18 오후 4 53 25" src="https://github.com/user-attachments/assets/9feec3ef-296e-4642-abd5-8866960d8cd3" />

#### 2. DBpia

- 국내 논문 기반 리서치
- 전공 과목이나 이론적 뒷받침이 필요할 때 사용 가능

<img width="400" height="390" alt="스크린샷 2025-07-18 오후 4 42 43" src="https://github.com/user-attachments/assets/5551f6d3-cac0-4a5a-b47c-f7b45b5af2a3" />

<img width="400" height="901" alt="스크린샷 2025-07-18 오후 4 42 50" src="https://github.com/user-attachments/assets/b8742263-c7c1-4f20-a8c5-f3ee3973e455" />

#### 3. Phind

- 개발자용 Perplexity 느낌
- 실무 코드, CS 개념, 레퍼런스를 실전 위주로 찾아줌
- 출처: https://yozm.wishket.com/magazine/detail/1944/

## 7/21 ~ 7/25 - Team 91

## 1주차 릴레이 프로젝트를 하며 느낀점

### J064 김재민

1. github action을 통해 내가 원하는 배포, 수정 등 거의 모든 것들을 자동화 할 수 있구나!
2. 2일차에 배운 linux관련 지식이 많이 도움이 되었다. github action을 ubuntu 환경에서 하기에!
3. 어떻게 보면, 나만의 mcp 서버? 를 만든 느낌이든다..! 내가 원하는 파일을 만들어 gist에 업로드 까지 자동화 해주다니!!
4. Ai를 통해 요약뿐만 아니라 여러 데이터를 수집, 수정, 생성 모든 분야에서 재생산하여 내가 만든 데이터와 관점을 비교할 수 있겠다.

### J112 박수완

1. 내가 정리한 학습 내용을 AI에게 보여주고 피드백을 받아보니 꽤 뿌듯했다. 단순히 칭잔을 하는 말을 넘어서 구체적으로 어떤 부분이 인상 깊었는지 짚어주니까, 내가 어떤 식으로 공부하면 좋은지도 감이 왔다. 내가 스스로를 칭찬하지 못할 때, AI의 객관적인 응원이 큰 힘이 될 수도 있다는 걸 느꼈다. 정보를 잘 표현하는 능력, 중요한 포인트를 요약한 부분, 학습 태도에 대한 칭찬을 받을 때 내가 성장하고있는걸 체감할 수 있었다.. 앞으로도 학습 정리를 이렇게 리뷰받는 방식으로 마무리해보면 좋을 것 같다.

2. 오늘의 기분을 이미지로 표현해보자는 말에 처음엔 조금 멍해졌지만,생각보다 이 과정이 재밌었다. 말로 표현하기 어려운 감정이나 만족감, 혹은 약간의 지침 같은 걸 이미지 한 장으로 정리하니까 뭔가 감정도 정돈되는 느낌이었다.
   특히 내가 선택한 이미지가 README에 들어간 걸 보면서 “오늘 하루, 이만하면 잘 살았다”는 기분이 들었다. 그냥 단순히 과제를 끝내는 게 아니라, 그 날의 나를 기록하고 정리하는 한 장면이 된 것 같았다.

### J261 지현동

1. 퀘스트2를하면서 그날 하루를 더 인상깊게 기억할 수 있었습니다. 주간회고할때 그날의 감정과 기억을 가져와서 더 자세하게 피드백할 수 있을 것 같습니다.
2. 퀘스트 4를 수행하면서는 의식적으로 AI답변의 레퍼런스를 참고하여서, AI 답변을 필터링 없이 받아드리는 것이 아니라, 분별력있게 받아드리는 연습을 할 수 있었습니다.
3. 다른 분들의 미션 수행을 보면서, 반성도하고, 좋은 아이디어도 얻어갈 수 있었습니다.

---

### J261\_지현동

- 수락한 퀘스트:
  - 퀘스트 2. 이미지 수집
    > 어떤 감정을 가지고 살아갔나 그림일기를 남기면, 주간 피드백을 작성할 때 더 생생하게 한 주의 피드백을 할 수 있을 것 같다.
  - 퀘스트 4. AI 자료 추천
    > AI 답변을 검증없이 받아드리곤 하는데, 이러한 버릇을 의식적으로 고치기 위한 좋은 루틴이 될 수 있을 것 같다.


<details>
<summary>⚓ 수행한 퀘스트 펼쳐 보기/닫기</summary>
<div markdown="1">

### 퀘스트 2.

<img width="1072" height="1332" alt="릴프퀘스트2" src="https://gist.github.com/user-attachments/assets/ca01ee35-4a75-4d79-8841-a26c52dbc489" />

### 퀘스트 4.
#### day6
- [MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Advanced_JavaScript_objects/Object_prototypes)
- [javascript.info](https://ko.javascript.info/)
- [W3school](https://www.w3schools.com/js/js_objects.asp)
- [You Don't know JS](https://github.com/getify/You-Dont-Know-JS/tree/2nd-ed)
- [모던 자바스크립트 Deep Dive](https://poiemaweb.com/)
- [블로그](https://velog.io/@radin/prototype)

#### day7

- [Understanding and Characterizing Mock Assertions in Unit Tests](https://arxiv.org/pdf/2503.19284)
- [Test Assertion Guide](https://www.w3.org/2006/03/test-assertion-guide)
- [What is Mocking? An Introduction to Test Doubles](https://www.geeksforgeeks.org/software-testing/what-is-mocking-an-introduction-to-test-doubles/)
- [Test Runner](https://zetcode.com/terms-testing/test-runner/)
- [The Linux Kernel Index Nodes](https://www.kernel.org/doc/html/latest/filesystems/ext4/inodes.html)
- [ext4 Data Structures and Algorithms](https://www.kernel.org/doc/html/latest/filesystems/ext4/)
- [FAT Filesystem](https://elm-chan.org/docs/fat_e.html#notes)
- [windows NT file system](https://ntfs.com/ntfs_basics.htm)
- [NTFS overview](https://learn.microsoft.com/en-us/windows-server/storage/file-server/ntfs-overview)
- [ext4 블로그 설명](https://ddongwon.tistory.com/66)

#### day8
- [Curry and Function Composition](https://medium.com/javascript-scene/curry-and-function-composition-2c208d774983)
- [currying-linkedin](https://www.linkedin.com/advice/0/what-currying-functional-programming-how-can-you-bfyhe)
- [What is currying in JavaScript?](https://blog.logrocket.com/understanding-javascript-currying/)

#### day9
- [Publisher-Subscriber pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/publisher-subscriber)
- [Ably: What is Pub/Sub?](https://ably.com/topic/pub-sub)
- [What is Pub/Sub Architecture?](https://www.geeksforgeeks.org/system-design/what-is-pub-sub/)

</div>
</details>


### J064 김재민 🤿 (퀘스트 완료!✅)

#### 수락한 퀘스트 :

퀘스트 3 : 미션 `README` 내용을 요약해 후속 모험가에게 전하라

<details>
<summary>🚀수행한 퀘스트 펼쳐 보기/닫기</summary>
<div markdown="1">
필요한 단계 설명

1. github repository 생성
2. 자동화 하는 코드 작성
3. github action 세팅

#### 1. github repository 생성

https://github.com/jammin94/github-action-auto-summarize-readme.md/tree/main
생성완료!

#### 2. 자동화 하는 코드 작성

1. 나의 Gist목록을 모두 불러온다
2. 그 중 Description의 특정 단어 (e.g. Day01)이 포함된 Gist를 찾는다.
3. 그 Gist의 README.md의 RAW 데이터를
4. gemini에게 요약을 request, 답변을 response로 받는다.
5. Summarize.md 파일을 해당 gist에 업로드한다.

구현 상세

- axios를 통한 HTTP 통신 구현
- Google Generative AI 라이브러리를 통한 gemini 통신 구현
- github action에서의 환경변수를 통한 민감 정보 캡슐화

index.js

```javascript
// index.js

const axios = require('axios'); // HTTP 요청을 위한 라이브러리
const { GoogleGenerativeAI } = require('@google/generative-ai'); // Google Generative AI 라이브러리 추가

// --- 환경 설정 (환경 변수 또는 명령줄 인자 사용) ---
const GITHUB_TOKEN = process.env.GH_PAT_GIST;
const GEMINI_API_KEY = process.env.GEMINI_API_KEY;
const GITHUB_USERNAME = process.env.GH_USERNAME;

// 명령줄 인자에서 GIST_DESCRIPTION_FILTER 가져오기 (인덱스 2가 첫 번째 사용자 정의 인자)
// 명령줄 인자가 없으면 환경 변수(secrets)에서 가져오도록 폴백
const GIST_DESCRIPTION_FILTER = process.argv[2] || process.env.GIST_DESCRIPTION_FILTER;
// process.argv[0]은 node 경로, process.argv[1]은 스크립트 파일 경로

// --- API 클라이언트 초기화 ---
const githubAxios = axios.create({
  baseURL: 'https://api.github.com',
  headers: {
    Authorization: `token ${GITHUB_TOKEN}`,
    Accept: 'application/vnd.github.v3+json',
  },
});

const genAI = new GoogleGenerativeAI(GEMINI_API_KEY);

// Gist 목록 가져오기
async function getUserGists(username) {
  try {
    const response = await githubAxios.get(`/users/${username}/gists`);
    return response.data;
  } catch (error) {
    console.error('Error fetching Gists:', error.response ? error.response.data : error.message);
    throw error;
  }
}

// RAW 내용 가져오기
async function getRawContent(url) {
  try {
    const response = await axios.get(url);
    return response.data;
  } catch (error) {
    console.error(`Error fetching raw content from ${url}:`, error.response ? error.response.data : error.message);
    throw error;
  }
}

// Gemini로 텍스트 요약하기
async function summarizeTextWithGemini(text) {
  try {
    const model = genAI.getGenerativeModel({ model: 'gemini-2.0-flash' });

    const prompt = `다음 README.md 내용을 요약해 주세요. 주요 목적, 핵심 기능, 사용 방법에 중점을 두세요. 요약은 마크다운 형식으로 제공하고, 약 3-5문장으로 간결하게 작성해 주세요:\n\n${text}`;

    const result = await model.generateContent(prompt);
    const response = await result.response;
    return response.text();
  } catch (error) {
    console.error('Error summarizing with Gemini:', error.response ? error.response.data : error.message);
    return null;
  }
}

// Gist 파일 업데이트
async function updateGist(gistId, filename, content) {
  try {
    const response = await githubAxios.patch(`/gists/${gistId}`, {
      files: {
        [filename]: {
          content: content,
        },
      },
    });
    return response.data;
  } catch (error) {
    console.error(
      `Error updating Gist ${gistId} with ${filename}:`,
      error.response ? error.response.data : error.message
    );
    throw error;
  }
}

async function main() {
  // 필수 환경 변수 및 필터 문자열 확인
  if (!GITHUB_TOKEN) {
    console.error('오류: GH_PAT_GIST 환경 변수가 설정되어야 합니다.');
    return;
  } else if (!GEMINI_API_KEY) {
    console.error('오류: GEMINI_API_KEY 환경 변수가 설정되어야 합니다.');
    return;
  } else if (!GITHUB_USERNAME) {
    console.error('오류: GH_USERNAME 환경 변수가 설정되어야 합니다.');
    return;
  }
  if (!GIST_DESCRIPTION_FILTER) {
    console.error('또한, GIST_DESCRIPTION_FILTER 값이 명령줄 인자 또는 환경 변수로 제공되어야 합니다.');
    console.error('예시: node index.js "원하는 필터 문자열"');
    return;
  }

  console.log(`필터링할 Gist 설명: "${GIST_DESCRIPTION_FILTER}"`); // 어떤 필터로 동작하는지 확인용 로그

  try {
    const allGists = await getUserGists(GITHUB_USERNAME);

    const targetGists = allGists.filter(
      (gist) => gist.description && gist.description.includes(GIST_DESCRIPTION_FILTER)
    );

    if (targetGists.length === 0) {
      console.log(`설명에 "${GIST_DESCRIPTION_FILTER}" 문자열이 포함된 Gist를 찾을 수 없습니다.`);
      return;
    }

    for (const gist of targetGists) {
      const gistId = gist.id;
      console.log(`Gist 처리 중: ${gistId} - ${gist.description}`);

      let readmeContent = null;
      let readmeFilename = null;

      for (const filename in gist.files) {
        if (filename.toLowerCase() === 'readme.md') {
          readmeFilename = filename;
          console.log(`  README.md 찾음: ${filename}`);
          try {
            readmeContent = await getRawContent(gist.files[filename].raw_url);
            break;
          } catch (error) {
            console.error(`  ${filename} 내용 가져오기 오류: ${error.message}`);
            readmeContent = null;
          }
        }
      }

      if (readmeContent) {
        const summaryContent = await summarizeTextWithGemini(readmeContent);
        if (summaryContent) {
          const summaryFilename = 'Summary.md';
          console.log(`  ${readmeFilename}에 대한 요약 생성 중. Gist에 ${summaryFilename} 업데이트.`);
          try {
            await updateGist(gistId, summaryFilename, summaryContent);
            console.log(`  Gist ${gistId}에 ${summaryFilename} 성공적으로 업데이트.`);
          } catch (error) {
            console.error(`  Gist ${gistId} 업데이트 오류: ${error.message}`);
          }
        } else {
          console.log(`  ${readmeFilename}에 대한 요약 생성 실패.`);
        }
      } else {
        console.log(`  Gist ${gistId}에서 README.md를 찾을 수 없거나 내용을 가져올 수 없습니다.`);
      }
    }
  } catch (error) {
    console.error('메인 함수 오류:', error.message);
  }
}

main();
```

#### 3. github action 세팅

1. 해당 코드가 있는 repository에 **actions** 에서 **new workflow** 생성
2. 자동화 할 yml파일 생성 후 작성

```yml
name: Gist README 요약 (설명 필터링 - Node.js - Gemini API)

on:
workflow_dispatch: # GitHub UI에서 수동 실행 시 입력 필드 사용
  inputs:
    description_filter: # 수동 실행 시 사용자로부터 직접 입력받음
      description: 'Gist description filter string'
      required: true
      default: ''

schedule: # 스케줄링하여 특정 필터 문자열로 주기적 실행 가능
  - cron: '0 0 * * *' # 매일 자정 UTC에 실행 (원하는 대로 조절)

jobs:
summarize:
  runs-on: ubuntu-latest
  steps:
    - name: 저장소 체크아웃
      uses: actions/checkout@v4

    - name: Set up Node.js
      uses: actions/setup-node@v4
      with:
        node-version: '18'

    - name: Install dependencies
      run: |
        npm install axios @google/generative-ai

    - name: Run Gist Summarizer Script
      env:
        GH_PAT_GIST: ${{ secrets.GH_PAT_GIST }}
        GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
        GH_USERNAME: ${{ secrets.GH_USERNAME }}
      run: |
        FILTER_ARG="${{ github.event.inputs.description_filter || secrets.GIST_DESCRIPTION_FILTER }}"
        if [ -z "$FILTER_ARG" ]; then
          echo "Error: GIST_DESCRIPTION_FILTER not provided via input or secret."
          exit 1
        fi
        node index.js "$FILTER_ARG"
```

- 작성 완료 시 자동으로 repository에 .github/workflows/[파일명].yml 생성 됨!

3. 해당 workflow를 description에 argument로, 내가 요약하고자 하는 gist의 description을 넣고 실행
   - 예를 들어, description에 'Day01'이 포함되어 있다면, Day01를 포함하여 실행하기
4. repository에 summary.md 파일 생성 확인하기
   <img width="987" height="300" alt="image" src="https://gist.github.com/user-attachments/assets/36411fce-000d-4a9d-bedf-f05bc9a1b72c" />

</div>
</details>

---

### J112 박수완

선택한 퀘스트 1. 칭찬받기

- 학습한 내용을 스스로 정리하고 AI에게 피드백을 요청하면서 내가 어떤 부분을 잘했는지 확인할 수 있을거 같습니다.
- AI로부터 긍정적인 피드백을 받는 경험은 성취감을 높이고 다음 학습에 대한 **동기부여**를 통해 더 집중할 수 있을거 같다.
- 내가 정리한 내용이 AI에게 어떻게 보이는지를 확인함으로써 **설명력과 표현력**을 되돌아볼 수 있습니다.

선택한 퀘스트 2. 이미지 수집

- 하루의 감정이나 회고를 **텍스트가 아닌 이미지로 표현**하는 시도는 창의적이며 재미있는 마무리가 될 수 있습니다.
- 단조로운 학습 기록에 시각적 요소를 더함으로써 더 미션에 몰입할 수 있을거같다

<details>
<summary>Ⓜ️수행한 퀘스트 펼쳐 보기/닫기</summary>
<div markdown="1">

## 퀘스트 1

<img width="700" height="1000" alt="Image" src="https://buly.kr/15PCrdD" />

## 퀘스트 2

<img width="700" height="1000" alt="Image" src="https://buly.kr/FsIrGH7" />

</div>
</details>
