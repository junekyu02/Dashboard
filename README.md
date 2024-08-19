# green up
### 탄소 인벤토리 기반 탄소 배출 감축 컨설팅 AI 서비스 

![greenup 로고](https://github.com/user-attachments/assets/988463c0-0289-4333-9dcc-6ed9893138e5)

최근 탄소 배출 저감과 환경 보호에 대한 관심이 높아지면서, 기업과 개인 모두에게 정확한 탄소 배출량 관리와 효율적인 저감 전략이 요구되고 있습니다. 

green up은 급격하게 증가하는 탄소 중립과 ESG(환경, 사회, 지배구조) 경영에 대한 요구를 반영하여, 중소기업(SME)들이 탄소 배출량을 체계적으로 관리하고 효과적인 감축 계획을 수립할 수 있도록 지원합니다.

사용자가 제공하는 탄소 배출량 데이터를 바탕으로, 탄소 인벤토리를 작성하고 그에 따른 감축 방안을 제안하는 **대시보드와 Solar LLM을 통한 AI 컨설팅 기능**을 제공합니다. green up를 통해 ESG의 복잡한 과제들을 직면한 중소기업에게 도움을 제공할 수 있습니다.


# 목차
1. [현재 개발 상황](#현재-개발-상황)
    1. [Chat 페이지](#chat-페이지)
2. [구현 기능](#구현-기능)
3. [추후 개발 방향](#추후-개발-방향)
4. [green up 사용법](#green-up-사용법)
    1. [green up 설치](#green-up-설치)
    2. [green up 실행](#green-up-실행)
5. [시연영상](#시연영상)
6. [팀원 구성 및 역할](#팀원-구성-및-역할)




## 현재 개발 상황
GreenUp의 웹 페이지는 사용자가 탄소 배출 데이터를 입력하고, 이를 바탕으로 한 맞춤형 분석 및 감축 계획을 제공하는 여러 기능을 포함합니다. 

#### 1. dashboard(홈) 페이지

ai chat페이지 사용자가 업로드한 엑셀 파일을 통해 AI가 데이터를 분석한 후, 대시보드 페이지로 이동하여 분석 결과를 시각적으로 확인할 수 있습니다. 대시보드 페이지는 아래와 같은 기능을 제공합니다.

1. 총 탄소 배출량: 업로드된 데이터에서 계산된 총 탄소 배출량을 표시합니다. 이 값은 Scope 1, 2, 3 범위에서의 모든 배출량을 합산한 결과입니다.
2. 원형 차트 (Pie Chart): Scope 1, 2, 3 범위의 배출량을 시각적으로 보여줍니다. 각 범위의 비율을 쉽게 파악할 수 있습니다. 예를 들어, Scope 1은 고정 연소와 이동 연소, 공정 배출 등 직접 배출을 포함하며, Scope 2는 전기 및 증기 사용으로 인한 간접 배출을 포함합니다.
3. 막대 차트 (Bar Chart): 연도별 총 탄소 배출량 변화를 막대 차트로 시각화합니다. 이를 통해 사용자는 시간에 따른 탄소 배출량의 추이를 쉽게 파악할 수 있습니다.
4. 카테고리별 배출량: 고정 연소, 이동 연소, 공정 배출, 전기 사용, 증기 사용 등 각 카테고리별로 상세한 배출량을 제공합니다. 각 항목은 tCO2e (톤 CO2 환산량) 단위로 표시되며, 전체 배출량에서 차지하는 비율도 함께 제공합니다.
5. PDF 리포트 다운로드: 분석 결과를 PDF 형식으로 다운로드할 수 있는 기능을 제공합니다. 


## 구현 기능

1.Pandas: 데이터 처리 및 분석
2.XlsxWriter: Excel 파일 생성 및 수정
3.Matplotlib: 데이터 시각화
4.Flask: 웹 서버 프레임워크
5.React: 프론트엔드 개발
6.Chart.js: 프론트엔드 시각화


## 추후 개발 방향

- ai chat 페이지와 dashboard 페이지 연결 작업 (ai chat 처음 실행 시 엑셀 양식과 서비스 설명을 주는 방향으로 개발)
- 대시보드 pdf 다운로드(리포트 형식)
- 목표 배출량 설정 후 얼마나 절감/오버 했는지 보여주는 기능





## green up 사용법
1. green up 설치    

   ```
   git clone https://github.com/your-repo/greenup.git  
   cd greenup  
   ```

3. green up 실행
   
    ```
   poetry install
   poetry run python manage.py runserver

    ```
  서버가 실행되면, 브라우저에서 http://localhost:3000을 열어 GreenUp 웹 페이지에 접속할 수 있습니다.




## 시연영상




https://github.com/user-attachments/assets/88d45e6b-e065-4e74-ba61-eb13f9c55ad7







## 팀원 구성 및 역할

| [<img src="https://github.com/Drizzle03.png" width="100px">](https://github.com/Drizzle03) | [<img src="https://github.com/seulnan.png" width="100px">](https://github.com/seulnan) | [<img src="https://github.com/junekyu02.png" width="100px">](https://github.com/junekyu02) | [<img src="https://github.com/jakepro657.png" width="100px">](https://github.com/jakepro657) |
| :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: |
| [편유나](https://github.com/Drizzle03) | [김난슬](https://github.com/seulnan) | [백준규](https://github.com/junekyu02) | [김유빈](https://github.com/jakepro657) |
| PM <br> Design | Frontend | Backend | AI |


