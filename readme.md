# 🥗 NutriChef AI Assistant

**NutriChef AI Assistant**는 20년 차 영양교육 전문가이자 수석 셰프의 노하우를 결합한 **맞춤형 건강 레시피 & 영양 코칭 웹 애플리케이션**입니다.  
사용자가 보유한 식재료와 건강 관심사를 입력하면, AI가 최적의 영양 시너지와 조리법을 고려하여 3가지 맞춤형 레시피와 1분 건강 코칭을 제공합니다.

---

## ✨ 주요 기능 (Key Features)

1. **건강 관심사 맞춤 선택 (Health Goals)**
   - 다이어트/체중감량, 혈당/당뇨 관리, 혈압/심혈관, 피로회복/면역, 소화/장건강, 근육증량/고단백 등 다중 선택 가능.
2. **냉장고 파먹기 식재료 입력 (Ingredient Input)**
   - 쉼표(`,`)를 이용해 보유 식재료를 손쉽게 입력.
   - 원클릭 샘플 재료 조합 제공 (#기본 건강재료, #식단 관리용, #고기류 조합).
3. **20년 차 전문가 페르소나 기반 AI 코칭**
   - **💡 1분 건강 코칭**: 영양소 섭취 순서, 영양 흡수율을 극대화하는 조리 팁 제공.
   - **🍽️ 맞춤 레시피 3선**:
     - **Option 1**: 초간단 10분 요리 (시간 절약형)
     - **Option 2**: 영양 균형 요리 (영양 강화형)
     - **Option 3**: 이색 별미 요리 (맛·풍미 강화형)
4. **유연한 API 엔드포인트 지원 (Dual AI Engine)**
   - **Google Gemini API**: 기본 내장 엔진 지원 (`gemini-3-flash-preview`).
   - **OpenAI API**: 사용자 개인 OpenAI API Key 입력 지원 (브라우저 `LocalStorage` 안전 보관).
5. **감각적인 내추럴 디자인 & 모바일 최적화**
   - Tailwind CSS 기반 내추럴 그린 & 웜 베이지 톤의 편안한 UI/UX.
   - 반응형 카드 레이아웃 및 로딩 스피너 제공.

---

## 🛠️ 기술 스택 (Tech Stack)

| 구분 | 사용 기술 |
| :--- | :--- |
| **Frontend** | HTML5, JavaScript (ES6+), Tailwind CSS (via CDN) |
| **Icons & Font** | FontAwesome 6, Pretendard 웹폰트 |
| **AI Integration** | Google Gemini API (`gemini-3-flash-preview`), OpenAI API (`gpt-4o-mini`) |
| **Data Storage** | Browser `LocalStorage` (API 키 저장용) |

---

## 🚀 시작하기 (Getting Started)

본 프로젝트는 단일 파일(`index.html`)로 작성되어 있어 **별도의 백엔드 서버나 빌드 과정 없이** 웹 브라우저에서 바로 실행할 수 있습니다.

### 1. 다운로드 및 실행

1. 프로젝트 디렉토리 내의 `index.html` 파일과 `README.md` 파일을 다운로드합니다.
2. `index.html` 파일을 웹 브라우저(Chrome, Edge, Safari 등)로 실행합니다.

### 2. API 키 설정 (선택 사항)

- 기본적으로 내장된 Gemini 엔진으로 동작합니다.
- 개인 **OpenAI API Key**를 사용하고 싶다면:
  1. 우측 상단의 **[API 키 설정]** 버튼 클릭.
  2. AI 제공자를 **OpenAI**로 변경.
  3. 보유한 `sk-...` API Key 입력 후 **[저장하기]** 클릭.

---

## 📖 사용 방법 (How to Use)

1. **건강 관심 분야 선택**: 원하는 건강 관리 목적을 1개 이상 선택합니다.
2. **식재료 입력**: 냉장고에 있는 식재료를 입력하거나 예시 버턴을 클릭합니다. (예: `계란, 두부, 양배추, 대파`)
3. **[맞춤 레시피 & 영양 조언 받기]** 버튼 클릭.
4. AI가 분석한 **1분 영양 코칭**과 **3가지 맞춤 레시피**를 확인하고 요리를 즐깁니다!

---

## 📂 프로젝트 구조 (Project Structure)

```text
.
├── index.html       # HTML, Tailwind CSS, JS가 통합된 단일 웹 앱 파일
└── README.md        # 프로젝트 안내 문서
```

---

## ⚠️ 라이선스 및 유의사항 (Disclaimer)

- **영양 정보 관련 유의사항**: 본 애플리케이션에서 제공하는 조언 및 레시피는 일반적인 건강 및 영양 정보에 기반하며, 전문적인 의학적 진단이나 치료를 대신할 수 없습니다.
- **보안**: 저장된 API Key는 오직 사용자의 브라우저(LocalStorage)에만 저장되며 외부 서버로 전송되지 않습니다.