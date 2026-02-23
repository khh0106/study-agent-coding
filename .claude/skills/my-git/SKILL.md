---
name: my-git
description: 이 레포의 커밋 메시지 컨벤션에 맞게 git commit을 수행한다.
allowed-tools: Bash, Read
disable-model-invocation: true
---

이 레포의 커밋 메시지 컨벤션에 맞게 git commit을 수행한다.

## 커밋 메시지 컨벤션

형식: `<타입>: <제목>`

| 타입 | 사용 상황 |
|------|-----------|
| `lecture` | 강의/영상 정리 문서 추가 |
| `docs` | 일반 문서 추가 및 수정 |
| `update` | 기존 문서 내용 보완/개선 |
| `fix` | 오타, 링크 오류 등 수정 |
| `refactor` | 문서 구조 또는 파일 정리 |
| `chore` | 설정 파일 수정 (.gitignore 등) |

**규칙:**
- 제목은 50자 이내, 현재형 명령조 사용 (예: `Add`, `Update`, `Fix`)
- 출처가 있는 경우 본문에 링크 포함

## 절차

1. `git status`와 `git diff`를 실행해 변경된 파일과 내용을 확인한다.
2. 변경 내용을 분석해 위 컨벤션에 맞는 타입과 제목을 결정한다.
3. 사용자에게 결정한 커밋 메시지를 보여주고 확인을 받는다.
4. 확인 후 `git add`와 `git commit`을 실행한다.

출처 URL이 있는 경우 커밋 본문에 포함한다.

$ARGUMENTS
