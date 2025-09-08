조직이 데이터 중심 방식으로 전환함에 따라 원시 정보에서 인사이트를 신속하게 해석하고 전달하는 능력은 중요한 기술입니다. Microsoft 365 Copilot의 분석 도구 에이전트는 사용자가 Excel 및 Forms와 같은 친숙한 도구 내에서 직접 데이터를 분석하고 시각화하여 이러한 능력을 발휘할 수 있도록 합니다. 이 랩에서는 분석 도구 에이전트를 사용하여 설문 조사, 스프레드시트 또는 설문 조사 결과 등 기존 데이터 세트를 이해하고 최소한의 노력으로 실행 가능한 인사이트로 전환하는 방법에 대한 실용적인 연습을 제공합니다.

이 시나리오 기반 연습에서는 분석 도구 에이전트를 사용하여 추세를 탐색하고, 변칙을 식별하고, 데이터 스토리텔링을 향상하는 시각적 개체를 생성하는 방법을 알아봅니다. 팀 성과, 고객 피드백 또는 운영 메트릭에 대해 보고하는 경우 이 랩에서는 원시 수치에서 명확한 요약 또는 이해 관계자가 바로 확인할 수 있는 차트로 전환하는 방법을 보여 줍니다. 이것은 AI 기반 지원을 통해 시간을 절약하고, 수동 작업을 줄이고, 분석 의사 결정에 대한 신뢰를 구축할 수 있는 강력한 방법입니다.

### 연습

새로운 디지털 작업 영역 플랫폼을 통해 부서 간 협업을 개선하기 위한 6주 간의 파일럿 프로그램인 "Project Nexus"라는 내부 회사 이니셔티브와 관련된 설문 조사 결과를 분석해야 합니다. 이 프로젝트에는 IT, HR, 마케팅 및 운영을 포함한 다양한 부서의 직원들이 참여했으며, 이들은 일상적인 커뮤니케이션, 문서 공유 및 작업 관리에 이 플랫폼을 사용하도록 요청받았습니다. 이 프로젝트의 목표는 생산성 향상, 커뮤니케이션 간소화 및 프로젝트 마감일 충족에 대한 플랫폼의 효율성을 평가하는 것이었습니다. 

파일럿이 끝난 후 참가자들은 프로젝트에 대한 만족도, 커뮤니케이션의 명확성과 효과, 제안된 타임라인 준수 및 새로운 시스템에 대한 전반적인 경험을 평가하기 위해 설문 조사를 실시했습니다. Microsoft 365 Copilot의 미리 빌드된 분석 도구 에이전트를 사용하여 Project Nexus의 설문 조사 결과를 살펴볼 계획입니다. 미리 빌드된 에이전트와 마찬가지로 사용자 지정 프롬프트를 입력하거나 에이전트의 시작 프롬프트를 사용할 수 있습니다. 분석 도구 에이전트의 시작 프롬프트는 정량적, 정성적, 시각화 분석 및 전반적인 프로젝트 인사이트와 권장 사항을 생성하도록 설계되었습니다.

다음 단계를 수행하여 분석 도구 에이전트가 Project Nexus와 관련된 설문 조사 결과를 해석하고 시각화하도록 지시합니다.

1. 다음 링크를 선택하여 [Project Nexus Survey Results](https://github.com/MicrosoftLearning/MS-4004-Empower-workforce-copilot-use-cases/raw/refs/heads/master/ResourceFiles/Project_Nexus_survey_results.xlsx)의 복사본을 다운로드합니다. 화면 상단의 **다운로드** 단추를 선택하여 파일을 디바이스로 다운로드하세요.
1. **Microsoft Edge**에서 새 탭을 열고 다음 URL을 입력합니다. [**https://M365copilot.com**](https://M365copilot.com) 
1. **Microsoft 365**의 **에이전트** 섹션 아래 탐색 창에 표시되는 **분석 도구** 에이전트를 선택합니다. 그렇지 않으면 탐색 창에서 **모든 에이전트**를 선택한 다음, **에이전트 저장소** 창의 **Microsoft에서 기본 제공** 섹션에서 **분석 도구**를 선택합니다. 
1. **Microsoft 365**에서 **분석 도구** 에이전트 창이 나타납니다. 프롬프트 필드에서 더하기 기호(**+**) 아이콘인 **콘텐츠 및 에이전트 추가** 아이콘을 선택합니다. 
1. 표시되는 메뉴에서 **이 디바이스에서 업로드**를 선택합니다. **파일 탐색기**에서 **다운로드** 폴더로 이동하고 이전에 다운로드한 **Project Nexus Survey Results** 파일을 선택한 다음, **열기**를 선택합니다. 
1. 프롬프트 필드에서 연결된 Project Nexus Survey Results 결과 파일 옆에 다음 프롬프트를 입력합니다. **이 스프레드시트를 분석하고 세 가지 주요 추세를 알려줘**.

   > [!NOTE]
   > 어떻게 분석 도구가 여러 Python 명령을 실행하여 추세의 최종 목록을 만드는지 확인합니다. 모든 명령이 완료되고 결과가 집계된 후 상위 세 가지 추세가 결정되는 데 1분 정도 기다려야 할 수 있습니다. 각 명령 아래에는 해당 명령의 결과에 대한 설명이 있습니다. 결과를 아래로 스크롤하여 상위 세 가지 추세를 확인합니다.
1. 각 범주를 자세히 살펴보려고 하므로 먼저 다음 프롬프트를 입력합니다. **각 설문 조사 범주의 평균 등급은 어떻게 되지**?
1. 테스트에서 에이전트는 빈 페이지처럼 보이는 항목을 반환합니다. 실제로는 빈 페이지가 아닙니다. 에이전트의 응답과 프롬프트 필드 사이에 나타나는 커다란 빈 공간 청크일 뿐입니다. 동일한 상황이 발생하면 세로 스크롤 막대를 사용하여 위로 스크롤하면 응답을 찾을 수 있습니다. 페이지 맨 아래로 스크롤하면 프롬프트 필드가 표시됩니다. 이 에이전트는 새로운 에이전트이므로 이 빈 공간은 해결해야 하는 문제로 보입니다. 반면, 이 연습을 수행할 때 이러한 불필요한 공백 문제가 해결되었을 수 있습니다. 두 경우 모두 결과를 검토합니다. 분석도구 에이전트가 "이러한 평균을 시각적으로 비교하고 싶나요?"와 같은 다음 단계를 제안하는 경우 프롬프트 필드에 **예**를 입력합니다(빈 공간 문제가 지속되는 경우 프롬프트 필드를 보기 위해 페이지 아래쪽으로 스크롤해야 함).
1. 다시 이전 프롬프트의 결과까지 스크롤하고(필요한 경우) 검토합니다.
1. 이 시점에서는 분석 도구 에이전트를 사용하여 원하는 시간만큼 자유롭게 설문 조사 결과를 분석하세요. 사용자 지정 프롬프트를 직접 입력하거나, 원하는 경우 수행하려는 분석 유형에 따라 다음 프롬프트를 시도해 보세요.
   - 정량적 분석 프롬프트:
      - **Which category received the highest average rating, and which received the lowest**?(가장 높은 평균 등급을 받은 범주와 가장 낮은 평균 등급을 받은 범주는 무엇인가요?)
      - **How many participants rated the project satisfaction as 4 or higher**?(프로젝트 만족도를 4 이상으로 평가한 참가자는 몇 명인가요?)
      - **What percentage of participants rated timeline adherence below 3**?(타임라인 준수 등급이 3 미만인 참가자 비율은 얼마나 되나요?)
      - **Can you identify any correlations between communication effectiveness and overall experience**?(커뮤니케이션 효율성과 전반적인 경험 간의 상관 관계를 파악할 수 있나요?)
   - 정성적 분석 프롬프트:
      - **Summarize the most common themes in the comments section**.(주석 섹션에서 가장 일반적으로 나타나는 주제를 요약하세요.)
      - **Are there any recurring concerns or suggestions mentioned in the comments**?(주석에 언급된 반복되는 우려 사항 또는 제안 사항이 있나요?)
      - **Identify any comments that mention issues with communication or timeline**.(커뮤니테이션 또는 타임라인과 관련된 문제를 언급하는 주석을 파악하세요.)
   - 인사이트 및 권장 사항 프롬프트:
      - **Based on the survey data, what are the top three strengths of Project Nexus**?(설문 조사 데이트에 따르면 Project Nexus의 주요 세 가지 강점은 무엇인가요?)
      - **What are the key areas for improvement suggested by the participants**?(참가자들이 제안한 주요 개선 영역은 무엇인가요?)
      - **Provide a summary report of the survey findings with actionable recommendations**.(설문 조사 결과의 요약 보고서와 실행 가능한 권장 사항을 제공하세요.)
   - 정량적 시각화 프롬프트:
      - **Generate a pie chart of overall ratings distribution**.(전체 등급 분포의 원형 차트를 생성하세요.)
      - **Create a bar chart comparing the average ratings for Project Satisfaction, Communication Effectiveness, Timeline Adherence, and Overall Experience**.(프로젝트 만족도, 커뮤니케이션 효율성, 타임라인 준수 및 전반적인 경험에 대한 평균 등급을 비교해서 보여 주는 가로 막대형 차트를 만드세요.)
      - **Plot a histogram of the satisfaction ratings to see the distribution of ratings**.(만족도 등급의 히스토그램을 그려 등급 분포를 확인하세요.)
      - **Generate a scatter plot to analyze the relationship between Communication Effectiveness and Overall Experience**.(커뮤니케이션 효율성과 전반적인 경험 간의 관계를 분석하는 산점도를 생성하세요.)
      - **Create a correlation heatmap for all numeric rating categories**.(모든 수치 등급 범주에 대한 상관 관계 열 지도를 만드세요.)
      - **Make a box plot for each rating category to show the range and quartiles**.(범위와 사분위수를 나타내는 각 등급 범주의 상자 그림을 그립니다.)
      - **Plot a line graph showing timeline adherence ratings over participants ordered by Participant ID**.(참가자 ID별로 정렬된 참가자에 대한 타임라인 준수 등급을 보여 주는 꺾은선형 그래프를 그립니다.)
