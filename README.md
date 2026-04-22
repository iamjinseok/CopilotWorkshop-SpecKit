# CopilotWorkshop-SpecKit

이 저장소는 GitHub Codespaces에서 SpecKit 워크플로우를 바로 실행하기 위한 최소 구성입니다.

## CodeSpace 실행 조건

- Java
- Maven
- GitHub SpecKit
- Spring Boot 실행환경

## 포함된 핵심 파일

- `.devcontainer/devcontainer.json`
  - Java 기반 컨테이너 이미지
  - Maven 사용 가능
  - Copilot/Copilot Chat 확장 자동 설치
  - Spring Boot 개발 확장 포함

## Codespaces에서 시작하기

### 개발 환경 설정 및 확인
1. GitHub 저장소에서 **Code > Codespaces > Create codespace on main** 선택

1. 환경 확인

```bash
java -version
mvn -version
uv --version
specify --version
```

### SpecKit을 활용하여 간단한 웹 어플리케이션 만들기

모델을 **GPT-5 mini**로 해주세요.

1. 터미널에서 specify 프로젝트 생성

```bash
specify init .
```

1. 프로젝트의 개발 지침을 생성

```text
/speckit.constitution
- 사용자가 리뷰하는 부분은 반드시 한글로 작성하세요.
```

1. 개발하고자 하는 내용 설정

```text
/speckit.specify
- 가운데 버튼을 누르면 카운터가 증가하는 웹 어플리케이션을 만들어주세요.
- 버튼은 보라색
- 카운터는 버튼 위에 크게 보이도록 표시하세요.
- 1 페이지만 있으면 됩니다.
```

1. 기술 스택과 아키텍처 결정

```text
/speckit.plan
- JAVA 사용
- Spring Boot 프레임워크 사용
- 프론트엔드를 구분하지 말고 빌드와 실행이 쉽게 구현
- maven 빌드 시스템 사용
```

1. 작업 계획 생성
AI가 무엇을 할 것인지 생각하는 단계
```text
/speckit.tasks
```

1. 구현 시작
AI가 실제로 구현하는 단계
```text
/speckit.implementation
```

## 라이선스

이 프로젝트는 [LICENSE](LICENSE)를 따릅니다.
