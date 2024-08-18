# green up
### 탄소 인벤토리 기반 탄소 배출 감축 컨설팅 AI 서비스 

![greenup 로고](https://github.com/user-attachments/assets/988463c0-0289-4333-9dcc-6ed9893138e5)

최근 탄소 배출 저감과 환경 보호에 대한 관심이 높아지면서, 기업과 개인 모두에게 정확한 탄소 배출량 관리와 효율적인 저감 전략이 요구되고 있습니다. 

green up은 급격하게 증가하는 탄소 중립과 ESG(환경, 사회, 지배구조) 경영에 대한 요구를 반영하여, 중소기업(SME)들이 탄소 배출량을 체계적으로 관리하고 효과적인 감축 계획을 수립할 수 있도록 지원합니다.

사용자가 제공하는 탄소 배출량 데이터를 바탕으로, 탄소 인벤토리를 작성하고 그에 따른 감축 방안을 제안하는 **대시보드와 Solar LLM을 통한 AI 컨설팅 기능**을 제공합니다. green up를 통해 ESG의 복잡한 과제들을 직면한 중소기업에게 도움을 제공할 수 있습니다.


# 목차
1. [green up 웹 페이지 기능](#green-up-웹-페이지-기능)
    1. [Chat 페이지](#chat-페이지)
2. [구현 기능](#구현-기능)
3. [green up 사용법](#green-up-사용법)
    1. [green up 설치](#green-up-설치)
    2. [데이터 다운로드 및 전처리](#데이터-다운로드-및-전처리)
    3. [green up 실행](#green-up-실행)
4. [시연영상](#시연영상)
5. [팀원 구성 및 역할](#팀원-구성-및-역할)


## green up 웹 페이지 기능
GreenUp의 웹 페이지는 사용자가 탄소 배출 데이터를 입력하고, 이를 바탕으로 한 맞춤형 분석 및 감축 계획을 제공하는 여러 기능을 포함합니다. 

#### 1. Chat 페이지
사용자가 처음 챗 페이지에 접속하면, 서비스 사용 방법에 대한 간단한 안내가 제공됩니다. 이 안내는 사용자가 AI 챗과 어떻게 상호작용할지, 그리고 어떤 정보가 필요한지를 설명합니다. 설명과 함께 엑셀파일 양식을 제공합니다. 엑셀파일을 다운받은 후 자신의 탄소 배출 데이터를 입력할 수 있습니다. 이 양식은 탄소 배출 인벤토리를 체계적으로 관리하기 위한 기본 틀을 제공합니다. 사용자가 완성된 **엑셀양식**을 챗 페이지에 업로드하면, AI는 이를 자동으로 인식하고 분석을 시작합니다. 업로드된 데이터는 AI가 탄소 배출량을 평가하고, Scope 1, 2, 3 등 다양한 범위에서의 배출량을 구체적으로 분석하는 데 사용됩니다.
이후 **대시보드 페이지**로 이동하여 업로드된 데이터를 바탕으로 AI가 생성한 분석 결과를 시각적으로 확인할 수 있습니다.

<div align="right">
###### 엑셀양식
    <a href="https://github.com/user-attachments/files/16650030/green.up.sample.xlsx">엑셀양식 다운로드</a>
</div>



## 구현 기능









## green up 사용법
1. green up 설치    
    ```
   git clone https://github.com/your-repo/greenup.git  
   cd greenup  

(예시임 깃에서 설치하는 법 넣기)

    ```
   
2. 데이터 다운로드 및 전처리

   제공된 Excel 템플릿을 사용하여, Scope 1, 2, 3에 따른 배출량 데이터를 작성합니다.

   데이터 파일을 /data 폴더에 저장한 후, 웹 페이지에서 업로드합니다.

   (ai chat에서 어떤식으로 하면되는지 설명하면 될 듯)

3. green up 실행


    ```
   poetry install
   poetry run python manage.py runserver

    ```
  서버가 실행되면, 브라우저에서 http://localhost:3000을 열어 GreenUp 웹 페이지에 접속할 수 있습니다.


## 시연영상



https://github.com/user-attachments/assets/e2c7b4a5-7cb9-45b8-92ff-70756df3150b






## 팀원 구성 및 역할

| [<img src="https://github.com/Drizzle03.png" width="100px">](https://github.com/Drizzle03) | [<img src="https://github.com/seulnan.png" width="100px">](https://github.com/seulnan) | [<img src="https://github.com/junekyu02.png" width="100px">](https://github.com/junekyu02) | [<img src="https://github.com/jakepro657.png" width="100px">](https://github.com/jakepro657) |
| :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: |
| [편유나](https://github.com/Drizzle03) | [김난슬](https://github.com/seulnan) | [백준규](https://github.com/junekyu02) | [김유빈](https://github.com/jakepro657) |
| PM <br> Design | Frontend | Backend | AI |

