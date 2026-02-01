# Azure Agent Tracing Demo

AI 에이전트 실행 과정을 시각화하는 데모 프로젝트입니다.

## 📋 개요

이 프로젝트는 3가지 방식으로 AI 에이전트의 작업 진행 상황을 표시하는 방법을 보여줍니다:

1. **Azure OpenAI** - 스트리밍 + Tool Calling 진행 상황 표시
2. **Microsoft Foundry Agent** - Run Steps 추적 및 표시
3. **Microsoft Agent Framework** - 멀티 에이전트 워크플로우 트레이싱

## 🚀 시작하기

### 1. 환경 설정

```bash
# 가상환경 생성
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
# .venv\Scripts\activate   # Windows

# 패키지 설치
pip install -r requirements.txt
```

### 2. 환경 변수 설정

```bash
cp .env.example .env
# .env 파일을 열고 Azure 자격 증명을 입력하세요
```

### 3. 노트북 실행

Jupyter Notebook 또는 VS Code에서 노트북을 실행하세요:

- `1_azure_openai.ipynb` - Azure OpenAI 스트리밍 + Tool Calling
- `2_foundry_agent.ipynb` - Microsoft Foundry Agent
- `3_agent_framework_workflow.ipynb` - Agent Framework 워크플로우

## 📁 프로젝트 구조

```
├── .env.example                    # 환경 변수 템플릿
├── .gitignore                      # Git 제외 파일
├── requirements.txt                # Python 패키지
├── 1_azure_openai.ipynb           # Azure OpenAI 데모
├── 2_foundry_agent.ipynb          # Foundry Agent 데모
└── 3_agent_framework_workflow.ipynb # Agent Framework 데모
```

## 🔧 필요 조건

- Python 3.10+
- Azure OpenAI 리소스
- Azure AI Foundry 프로젝트 (선택사항)
- Azure 자격 증명 (DefaultAzureCredential)

## 📚 참고 자료

- [Azure OpenAI 문서](https://learn.microsoft.com/azure/ai-services/openai/)
- [Azure AI Foundry 문서](https://learn.microsoft.com/azure/ai-studio/)
- [Agent Framework 문서](https://learn.microsoft.com/agent-framework/)

## 📝 라이선스

MIT License
