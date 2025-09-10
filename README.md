# 🚀 Azure OpenAI + Chainlit 고급 AI 모델 배포

Azure OpenAI Service의 최신 AI 모델들(GPT-5, Sora, o3 시리즈)을 활용한 차세대 AI 챗봇을 원클릭으로 배포하세요!

## ✨ 지원 모델

### 🧠 채팅 완성 모델
- **GPT-4o** (기본) - 최신 멀티모달 모델
- **GPT-4o Mini** - 빠르고 효율적인 경량 모델  
- **GPT-4 Turbo** - 고성능 텍스트 모델
- **🆕 GPT-5 Preview** - 차세대 언어 모델 (특별 액세스 필요)
- **🆕 o3-mini** - 고급 추론 모델 (경량)
- **🆕 o3-pro** - 최고 성능 추론 모델

### 🎬 비디오 생성 (선택)
- **🆕 Sora** - AI 비디오 생성 모델

### 📊 임베딩 모델  
- **text-embedding-ada-002** (기본)
- **text-embedding-3-large** (고급 모델 활성화 시)

## 🚀 원클릭 배포

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2F[YOUR_USERNAME]%2Fazure-chainlit-openai-deploy%2Fmain%2Fazuredeploy.json)

## ⚙️ 배포 파라미터

| 파라미터 | 기본값 | 옵션 | 설명 |
|---------|--------|------|------|
| **projectName** | chainlit-openai | - | 모든 리소스의 기본 이름 |
| **location** | eastus | eastus, westeurope, etc. | Azure 지역 |
| **chatModel** | gpt-4o | gpt-4o, gpt-5-preview, o3-pro 등 | 주 채팅 모델 |
| **enableSora** | false | true/false | Sora 비디오 생성 활성화 |
| **enableAdvancedModels** | false | true/false | GPT-5, o3 시리즈 활성화 |
| **modelCapacity** | 10 | 10, 20, 50, 100 | 모델 용량 (TPM 천 단위) |

## 🎯 모델별 특징 및 사용 사례

### 🤖 GPT-4o (권장 시작 모델)
```
✅ 텍스트, 이미지, 오디오 멀티모달
✅ 빠른 응답 속도  
✅ 높은 정확도
✅ 비용 효율적

사용 사례: 일반 채팅, 문서 분석, 이미지 해석
```

### 🧠 GPT-5 Preview (차세대!)
```  
🆕 더욱 향상된 추론 능력
🆕 복잡한 문제 해결
🆕 창의적 작업 특화
⚠️ 특별 액세스 권한 필요

사용 사례: 고급 연구, 창작, 복합 문제 분석
```

### 🔬 o3-pro (최강 추론!)
```
🧠 최고 수준의 수학적 추론
🧠 과학적 문제 해결
🧠 코딩 및 알고리즘 특화  
💰 높은 비용

사용 사례: 연구용 계산, 고급 프로그래밍, 수학 문제
```

### 🎬 Sora (비디오 생성)
```
🎥 텍스트로 고품질 비디오 생성
🎥 최대 60초 비디오 
🎥 1080p 해상도
⚠️ 높은 비용 및 특별 액세스 필요

사용 사례: 교육용 비디오, 프레젠테이션, 창작
```

## 🎮 실습 시나리오

### 🔰 기본 테스트 (GPT-4o)
```
"안녕하세요! Python으로 데이터 시각화를 해주세요"
"이 이미지에서 무엇을 볼 수 있나요?" (이미지 업로드)
```

### 🧠 고급 추론 (o3-pro)
```  
"복잡한 수학 문제를 풀어주세요: 최적화 문제"
"이 코드를 최적화하고 알고리즘을 개선해주세요"
"과학적 가설을 검증하는 실험을 설계해주세요"
```

### 🎬 비디오 생성 (Sora)
```
"고양이가 공원에서 뛰어노는 30초 비디오를 만들어주세요"
"미래 도시의 모습을 보여주는 비디오"
"교육용 애니메이션: 광합성 과정"
```

### 🚀 차세대 AI (GPT-5)
```
"창의적인 소설을 써주세요: SF 장르"  
"복합적인 비즈니스 전략을 수립해주세요"
"여러 학문을 융합한 혁신적 아이디어를 제안해주세요"
```

## 📊 성능 및 비용 비교

| 모델 | 속도 | 정확도 | 비용 | 특장점 |
|------|------|--------|------|---------|
| GPT-4o | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | $ | 균형 잡힌 성능 |
| GPT-4o Mini | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | $ | 빠르고 경제적 |
| GPT-5 Preview | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | $$$ | 최고 창의성 |
| o3-mini | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | $$ | 추론 특화 경량 |
| o3-pro | ⭐⭐ | ⭐⭐⭐⭐⭐ | $$$$ | 최강 추론 |
| Sora | ⭐⭐ | ⭐⭐⭐⭐ | $$$$$ | 비디오 생성 |

## 🛡️ 액세스 권한 안내

### 🔓 일반 액세스 (누구나 사용 가능)
- GPT-4o, GPT-4o Mini, GPT-4, GPT-4 Turbo
- text-embedding-ada-002

### 🔒 특별 액세스 필요 (신청 후 승인)
- **GPT-5 Preview**: [OpenAI 연구 프로그램](https://openai.com/research) 신청
- **o3 시리즈**: [Azure OpenAI 고급 모델 액세스](https://aka.ms/oai/access) 신청  
- **Sora**: [Sora 베타 프로그램](https://openai.com/sora) 신청

⚠️ 특별 액세스가 없는 상태에서 해당 모델을 선택하면 배포가 실패할 수 있습니다.

## 💰 예상 비용 (월간)

### 기본 구성 (GPT-4o)
```
🏗️ 인프라: ~$25-35
🤖 GPT-4o: ~$20-50 (사용량 기반)
📊 총합: ~$45-85/월
```

### 고급 구성 (o3-pro + Sora)
```
🏗️ 인프라: ~$25-35
🧠 o3-pro: ~$100-300 (사용량 기반)  
🎬 Sora: ~$200-500 (비디오 생성량 기반)
📊 총합: ~$325-835/월
```

## 🗑️ 리소스 정리

테스트 완료 후 비용 절약을 위해 리소스 정리:

```bash
# Azure CLI로 정리
az group delete --name [리소스-그룹-이름] --yes --no-wait

# 또는 Azure Portal에서 리소스 그룹 삭제
```

## ⚠️ 주의사항

- **지역 제한**: 최신 모델은 특정 지역에서만 지원 (US East, West Europe 권장)
- **할당량 제한**: 고급 모델은 할당량 신청이 필요할 수 있음
- **높은 비용**: o3-pro, Sora는 매우 높은 비용 발생 가능
- **액세스 승인**: GPT-5, o3, Sora는 사전 승인 필요
- **첫 로딩**: Container 이미지 다운로드로 2-3분 소요

## 🔄 모델 변경

배포 후 Azure Portal에서 다른 모델로 쉽게 변경 가능:

1. Azure OpenAI Service → 모델 배포
2. 새 모델 추가 배포
3. Container App 환경변수에서 `AZURE_OPENAI_DEPLOYMENT_NAME` 변경
4. Container App 재시작

## 📚 관련 문서

- [Azure OpenAI Service](https://docs.microsoft.com/azure/ai-services/openai/)
- [GPT-5 연구 문서](https://openai.com/research/gpt-5)
- [o3 시리즈 소개](https://openai.com/o3)
- [Sora 기술 문서](https://openai.com/sora)
- [Chainlit 공식 문서](https://docs.chainlit.io/)

## 🤝 기여하기

이 프로젝트 개선에 참여하세요:
- 🐛 버그 리포트: Issues 탭
- 💡 기능 제안: Discussions 탭  
- 🔧 코드 기여: Pull Requests

---

⭐ **이 리포지토리가 도움이 되셨다면 Star를 눌러주세요!**

🚀 **차세대 AI의 힘을 직접 체험해보세요!**