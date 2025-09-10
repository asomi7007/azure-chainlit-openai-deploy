# 🚀 Azure OpenAI + Chainlit 핸즈온 배포

Azure OpenAI Service와 Chainlit를 활용한 AI 챗봇을 **자동 고유 이름**으로 배포합니다.  
**리소스 그룹 중복 걱정 없이** 원클릭 배포 가능! 🎯

## ✨ 주요 기능
- 🤖 **Azure OpenAI GPT-4o** 최신 모델 활용
- 💬 **Chainlit** 기반 사용자 친화적 채팅 인터페이스  
- 📁 **파일 업로드** 및 분석 기능 (PDF, DOCX, 이미지)
- 🔧 **Code Interpreter** - 실시간 코드 실행
- 🔍 **File Search** - 업로드된 문서 검색
- ☁️ **Azure Container Apps**에서 서버리스 실행
- ✅ **자동 고유 명명** - 중복 이름 충돌 방지

## 🚀 원클릭 배포

**중복 걱정 없이 바로 배포하세요!**

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fasomi7007%2Fazure-chainlit-openai-deploy%2Fmain%2Fazuredeploy.json)

## 🎯 스마트 네이밍 시스템

### 자동 생성되는 리소스 이름 예시:
```
리소스 그룹: rg-chainlit-handson-a1b2c3d4
OpenAI 서비스: chainlit-ai-a1b2c3d4-140930
Container App: chainlit-app-a1b2c3d4-140930
Environment: chainlit-env-a1b2c3d4-140930
```

**✅ 장점:**
- 🔄 **완전 자동화** - 매번 다른 고유 이름
- ⚡ **즉시 배포** - 이름 충돌로 인한 실패 없음
- 🎯 **핸즈온 최적화** - 여러 참가자가 동시 배포 가능

## 📋 배포 파라미터

| 파라미터 | 기본값 | 설명 |
|---------|--------|------|
| baseName | chainlit | 모든 리소스의 기본 이름 |
| location | eastus | Azure 지역 (OpenAI 지원 보장) |

## 🎯 사용 방법

### **핸즈온 참가자용:**
1. **Deploy to Azure** 버튼 클릭 ⬆️
2. **기본값 그대로 사용** (변경 불필요!)
3. **리소스 그룹**: 새로 만들기 → `rg-chainlit-handson-[본인이니셜]`
4. **만들기** 클릭 → 10-15분 대기 ☕
5. **출력** 탭에서 Container App URL 확인
6. **URL 클릭** → AI 채팅 시작! 🎉

## 🧪 테스트 시나리오

### **🔰 기본 채팅**
```
"안녕하세요! Azure OpenAI에 대해 간단히 설명해주세요"
```

### **💻 코딩 테스트**
```
"Python으로 피보나치 수열을 생성하는 함수를 만들어주세요"
```

### **📊 데이터 분석**
```
"CSV 파일을 업로드하고 데이터를 분석해주세요"
```

### **🎨 창작 활동**
```
"미래 도시를 주제로 한 짧은 시를 써주세요"
```

## 💰 예상 비용

- **Azure OpenAI**: 사용량 기반 (GPT-4o 토큰당)
- **Container Apps**: ~$15-25/월 (vCPU 0.5, Memory 1GB)  
- **Log Analytics**: 무료 티어 포함

**총 예상: ~$20-30/월** (실제 사용량에 따라 변동)

## 🗑️ 리소스 정리 (중요!)

**테스트 완료 후 반드시 정리하세요:**

### **Azure Portal에서:**
1. **리소스 그룹** 검색
2. `rg-chainlit-handson-xxxxx` 선택
3. **리소스 그룹 삭제** 클릭
4. 그룹 이름 입력하여 확인 삭제

### **Azure CLI로:**
```bash
# 리소스 그룹 목록 확인
az group list --query "[?contains(name, 'chainlit')].name" -o table

# 특정 리소스 그룹 삭제
az group delete --name rg-chainlit-handson-xxxxx --yes --no-wait
```

## ⚠️ 핸즈온 주의사항

- ✅ **기본값 사용**: 파라미터 변경 불필요, 그대로 배포
- ✅ **지역 선택**: East US 권장 (OpenAI 지원 보장)
- ✅ **첫 로딩**: Container 이미지 다운로드로 1-2분 소요
- ✅ **정리 필수**: 테스트 후 리소스 그룹 삭제로 비용 절약

## 📚 관련 문서

- [Azure OpenAI Service](https://docs.microsoft.com/azure/ai-services/openai/)
- [Chainlit 공식 문서](https://docs.chainlit.io/)  
- [Azure Container Apps](https://docs.microsoft.com/azure/container-apps/)
- [Azure 가격 계산기](https://azure.microsoft.com/pricing/calculator/)

## 🤝 지원 및 문의

**문제 발생 시:**
- 🔧 [GitHub Issues](https://github.com/asomi7007/azure-chainlit-openai-deploy/issues)
- 📧 이메일 문의
- 💬 실시간 지원 (핸즈온 중)

---

⭐ **이 리포지토리가 도움이 되셨다면 Star를 눌러주세요!**

**🚀 중복 걱정 없는 스마트 배포로 AI의 미래를 체험하세요!**

---
**GitHub Repository**: https://github.com/asomi7007/azure-chainlit-openai-deploy/
