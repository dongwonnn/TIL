# ❓ 컨벤션을 왜 지켜야 할까

**컨벤션은 협약**이라는 의미처럼 여러 사람이 지켜야 할 **일종의 룰**입니다. 따라서 개발자들이 협업 과정에서 컨벤션을 지킨다면 다음과 같은 이점이 있습니다.

1. 더 좋은 **가독성**
2. 더 좋은 **유지 보수**
3. 더 좋은 **협업과 관리**

# 📄 커밋 컨벤션

커밋 컨벤션은 **git 커밋 메세지**를 위한 컨벤션입니다. git 커밋을 이용해 **더 나은 로그 가독성, 리뷰 프로세스, 코드 유지 보수**를 할 수 있습니다.

## 커밋 메세지 구조

커밋 메세지는 **제목, 본문, 꼬리말**로 구성되어 있고 각자 빈 줄을 두어 구분합니다. 제목을 제외한 나머지는 옵션이지만 웬만하면 지키고 싶어 옵션을 지웠습니다. ( `꼬리말은 제외` )

> 타입 : [#이슈 번호 - ] 제목
>
> 본문
>
> 꼬리말(옵션)

### 타입

커밋 메세지가 **어떤 의도**를 가진 메세지인지 알립니다.
**태그와 제목**으로 구성되어 있고 사용법은 **태그: 제목**의 형태입니다. (`: 뒤에만 space가 있다 !`)

**ex) Feat: Infinity Scroll 추가**

#### 태그 종류들

<table style="text-align : center;">
    <th>태그</th>
    <th>의도</th>
    <th>태그</th>
    <th>의도</th>
    <tr>
        <td style="color : red">✔️ Feat</td>
        <td style="color : red">새 기능 추가</td>
        <td style="color : red">✔️ Fix</td>
        <td style="color : red">버그 수정</td>
    </tr>
    <tr>
        <td style="color : red">✔️ Design</td>
        <td style="color : red">CSS, UI 변경</td>
        <td style="color : red">✔️ Style</td>
        <td style="color : red">포맷 변경 등 코드 수정이 없는 경우</td>
    </tr>
        <tr>
        <td style="color : red">✔️ Refactor</td>
        <td style="color : red">코드 리팩토링</td>
        <td style="color : red">✔️ Comment</td>
        <td style="color : red">주석 추가</td>
    </tr>
    </tr>
        <tr>
        <td style="color : red">✔️ Docs</td>
        <td style="color : red">문서 수정</td>
        <td>Test</td>
        <td>테스트 추가, 리팩토링</td>
    </tr>   
    </tr>
    <tr>
        <td style="color : red">✔️ Rename</td>
        <td style="color : red">파일명 수정, 이동</td>
        <td style="color : red">✔️Remove</td>
        <td style="color : red">파일 삭제</td>
    </tr>
    <tr>
        <td>Chore</td>
        <td>패키지 매니저 설정</td>
        <td>!HOTFIX</td>
        <td>급한 버그 수정</td>
    </tr>
    <tr>
        <td>!BREAKING</br>
        CHANGE</td>
        <td>커다란 API 변경</td>
        <td></td>
        <td></td>
    </tr>
</table>

### 제목

제목은 메세지의 **짧은 요약**입니다. 다음과 같은 규칙을 가집니다.

1. "고침", "추가", "변경" 등 **명령조**로 시작합니다. ( 영어의 경우 동사 원형 )
2. 총 글자는 **50자** 이내
3. 마지막에 **특수문자 삽입 X**
4. **개조식** 구문 ( 간결, 요점적인 서술 )

> Feat: "추가 Infinty Scroll 기능"

### 본문

본문은 다음과 같은 규칙을 가집니다.

1. 한 줄 당 **72자 내외**
2. **최대한 상세히 작성**
3. 어떻게보단 **무엇, 왜**에 중점적으로

> Feat: "추가 Infinity Scroll 기능"
>
> - react-intersection-observer 패키지 사용
> - intersection 관측 시 다음 page API 호출

### 꼬리말

1. **이슈 트래커 ID**를 작성합니다. `"유형: #이슈 번호"`
2. 여러 개의 이슈 번호는 **쉼표**로 구분합니다.
3. 이슈 트래커 **유형**
   - **Fixes**: 이슈 수정 중 ( 아직 미해결 )
   - **Resolves**: 이슈 해결
   - **Ref**: 참고할 이슈
   - **Related to**: 해당 커밋과 관련된 이슈 번호 ( 아직 미해결 )

> Feat: "추가 Infinity Scroll 기능"
>
> - react-intersection-observer 패키지 사용
> - intersection 관측 시 다음 page API 호출
>
> Reslves: #321

# 참고 사이트

#### 🔗[참고 1](https://overcome-the-limits.tistory.com/entry/%ED%98%91%EC%97%85-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-%EA%B8%B0%EB%B3%B8%EC%A0%81%EC%9D%B8-git-%EC%BB%A4%EB%B0%8B%EC%BB%A8%EB%B2%A4%EC%85%98-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0)

#### 🔗[참고 2](https://meetup.toast.com/posts/106)
