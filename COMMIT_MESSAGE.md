<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Commit%20Message%20Rules&fontSize=60&animation=fadeIn&fontAlignY=38&descAlignY=51&descAlign=62)

**🦁 한림대 멋사 아기사자🦁**들의 원활한 협업을 위한 commit 규칙을 정리해두었습니다.

</div>

---

# 🧾 커밋 메시지 형식 (Formats for Commit Messages)

커밋 메시지는 **제목(Subject), 본문(Body), 꼬리말(Footer)** 세 가지로 나뉘며, 각 파트는 **공백 줄**로 구분합니다.

```
type(타입): title(제목)   ← Subject

Body(본문, 생략 가능)

Footer(생략 가능)
```

---

## 🔖 Message Tag (태그)

타입은 **태그: 제목** 형태로 쓰고, 태그는 **영어**, **첫 글자 대문자**로 합니다. **콜론(:) 뒤에 공백**을 넣어주세요.

| 태그 이름 | 태그 설명 |
|:---:|:---|
| Feat | 새로운 기능 추가 |
| Fix | 버그 수정 |
| !BREAKING CHANGE | 커다란 API 변경의 경우 |
| !HOTFIX | 급한 치명적 버그 수정 |
| Build | 빌드 관련 파일 수정 |
| Design | CSS를 포함 UI 디자인 변경 |
| Docs | 문서(문서 추가, 수정, 삭제) |
| Style | 스타일(코드 형식, 세미콜론 등 – 비즈니스 로직 변경 없음) |
| Refactor | 코드 리팩토링 |
| Comment | 필요한 주석 추가 및 변경 |
| Test | 테스트 코드 추가·수정·삭제 (비즈니스 로직 변경 없음) |
| Rename | 파일, 폴더명 이름 수정 |
| Remove | 파일, 폴더 삭제 |

---

## ▫️ Subject(제목) 규칙

- 첫 글자는 **대문자**, 제목 끝에는 **마침표(.)를 붙이지 않는다.**
- 영문 기준 **최대 50자** 내로 작성한다.
- **동사 원형**을 사용해 **명령문** 형태로 쓴다. (예: Add, Fix, Update)
- 본문과 제목은 **공백 줄**로 구분한다.

#### 예시 (Example of Subject)

```
Fix: 축제 관리자만 부스 목록에서 모든 데이터를 확인하도록 수정
```

---

## ▫️ Body(본문) 규칙

- **선택 사항**이므로 모든 커밋에 쓸 필요는 없다.
- 한 줄은 **72자**를 넘지 않도록 한다.
- **무엇을, 왜** 변경했는지 자세히 쓰고, 가능하면 **어떻게**도 간단히 적는다.
- 커밋의 **이유**를 적을 때도 본문을 활용한다.

#### 예시 (Example of Body)

```
축제 관리자만 부스 목록에서 모든 데이터를 확인하도록 수정
  - BoothMapView.vue: 관리자 유형에 따른 부스 페이지에 대한 권한을 부여함.
```

---

## ▫️ Footer(꼬리말) 규칙

- **선택 사항**이며, 관련 **이슈 번호**를 붙일 때 사용한다. (예: Fixes #1, #2)
- 키워드: **Closes**, **Fixes**, **Resolves**, **Ref**, **Related to** 등.
  - **해결** : 해결한 이슈 ID  
  - **관련** : 해당 커밋에 관련된 이슈 ID  
  - **참고** : 참고할 만한 이슈 ID  

#### 예시 (Example of Footer)

```
해결: #123
관련: #321
참고: #222
```

---

## ▫️ 전체 커밋 메시지 예시 (Full Example)

```
Fix: 축제 관리자만 부스 목록에서 모든 데이터를 확인하도록 수정 (#123)

축제 관리자만 부스 목록에서 모든 데이터를 확인하도록 수정
  - BoothMapView.vue: 관리자 유형에 따른 부스 페이지에 대한 권한을 부여함.

해결: #123
```

---

## ▫️ 적절한 커밋 메시지 예시

- **태그를 사용**하고, **무엇을 했는지** 한 줄에 드러나게 작성하면 좋습니다.
- 팀원이 히스토리만 보고도 변경 내용을 파악할 수 있도록 작성합니다.

---

## ▫️ 부적절한 커밋 메시지 예시

다음과 같은 메시지는 피하는 것이 좋습니다.

- `수정`, `업데이트`, `asdf`, `123` 등 **내용을 알 수 없는 한두 단어**
- **태그 없이** 제목만 나열
- **무엇을/왜 바꿨는지** 전혀 드러나지 않는 문장

이렇게 쓰면 다른 개발자가 어떤 작업을 했는지 파악하기 어렵습니다.

---

## 🙇 Written by

| LIKELION-HALLYM |
|:---:|
| 2026년 1학기 한림대 멋쟁이사자처럼 |

---

## 📎 References

- [Github Commit Message Rules - Junhyunny's Devlogs](https://junhyunny.github.io/information/github/git-commit-message-rule/#example-of-subject)
- [LikeLion-at-DGU : README](https://github.com/LikeLion-at-DGU/.github/blob/main/profile/README.md)
