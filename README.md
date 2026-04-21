# CopilotWorkshop-SpecKit

이 저장소는 GitHub Codespaces에서 SpecKit 워크플로우를 바로 실행하기 위한 최소 구성입니다.

## CodeSpace 실행 조건

- Java 21
- Maven
- GitHub SpecKit slash commands (`/specify`, `/plan`, `/tasks`, `/implement`)
- Spring Boot 실행환경

## 포함된 핵심 파일

- `.devcontainer/devcontainer.json`
  - Java 21 기반 컨테이너 이미지
  - Maven 사용 가능
  - Copilot/Copilot Chat 확장 자동 설치
  - Spring Boot 개발 확장 포함
- `.github/prompts/specify.prompt.md`
- `.github/prompts/plan.prompt.md`
- `.github/prompts/tasks.prompt.md`
- `.github/prompts/implement.prompt.md`

## Codespaces에서 시작하기

1. GitHub 저장소에서 **Code > Codespaces > Create codespace on main** 선택
2. Codespace가 열리면 Copilot Chat 창 열기
3. 아래 순서로 실행

```text
/specify Spring Boot 기반 Counter 웹앱 요구사항 문서를 만들어줘
/plan 방금 생성한 spec을 기준으로 구현 계획을 작성해줘
/tasks plan 기준으로 구현 작업을 체크리스트로 분해해줘
/implement 가장 우선순위가 높은 미완료 작업 1개를 구현해줘
```

## 환경 확인

Codespace 터미널에서 아래만 확인하면 됩니다.

```bash
java -version
mvn -version
```

Copilot Chat에서 `/specify` 자동완성이 보이면 SpecKit 사용 준비가 완료된 상태입니다.

## 라이선스

이 프로젝트는 [LICENSE](LICENSE)를 따릅니다.
