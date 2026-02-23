---
name: note
description: Claude Code 학습 내용을 claude-code-guide/ 폴더에 마크다운으로 정리. 학습 내용을 기록하거나 정리 요청 시 사용.
argument-hint: <주제 또는 파일명> (예: /note Hooks, /note claude-code-guide/04.md)
allowed-tools: Read, Write, Edit, Glob
disable-model-invocation: true
---

오늘 학습한 Claude Code 내용을 `claude-code-guide/` 폴더에 정리한다.

## 절차

1. `claude-code-guide/` 폴더의 기존 파일 목록을 확인한다.
2. `$ARGUMENTS`를 주제로 하는 파일이 이미 있으면 해당 파일에 내용을 추가한다.
   없으면 새 파일을 생성한다. (파일명 예: `hooks.md`, `slash-commands.md`)
3. 다음 형식으로 내용을 작성한다:

```markdown
# 주제

> 작성일: YYYY-MM-DD

## 핵심 개념

- 개념 1
- 개념 2

## 사용법

\`\`\`bash
예시 코드
\`\`\`

## 실습 메모

직접 해본 것, 주의사항, 팁 등
```

4. 현재 대화 내용을 바탕으로 핵심만 간결하게 정리한다.
5. 저장 후 파일 경로를 알려준다.

$ARGUMENTS
