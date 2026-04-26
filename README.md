# JMeter Test Plans

This repository contains various Apache JMeter test plans (`.jmx`) and related data files used for performance testing, feature demonstrations, and JMeter study.

## 📂 Files and Scenarios

### 1. Feature Demonstrations
These test plans are designed to demonstrate specific capabilities and components within JMeter:

*   **`JMeter Correlation Advanced 30.jmx`**
    *   Contains 30 advanced correlation exercises and examples of various **Post-Processors (Extractors)**. Demonstrates accurate extraction of dynamic values using Regular Expressions, JSON Path, XPath, CSS Selectors, etc.
*   **`JMeter_Correlation_Examples.jmx`**
    *   Provides foundational examples of correlation techniques to extract and utilize dynamic response data in subsequent requests.
*   **`JMeter Groovy Scripting Demo.jmx`**
    *   Demonstrates the use of **JSR223 Samplers/PreProcessors/PostProcessors** with Groovy scripting for custom logic, data manipulation, and advanced test scenarios.
*   **`JMeter-logic-controllers.jmx`** & **`JMeter_Logic_Controller_sample.jmx`**
    *   Comprehensive demonstrations of JMeter's **Logic Controllers** (If, While, Switch, ForEach, Random, Throughput, etc.). Showcases how to dynamically control the test execution flow based on variables.
*   **`JMeter-module.jmx`**
    *   Illustrates the use of the **Module Controller** and **Test Fragments** to create modular, reusable test components, improving maintainability of complex test plans.
*   **`JMeter_Thread_Group.jmx`** & **`threadgroup_http_example.jmx`**
    *   Showcases different configurations of **Thread Groups** (e.g., Standard Thread Group, Concurrency Thread Group, Stepping Thread Group) and HTTP Request samplers to simulate diverse load generation patterns.

### 2. Petstore Application Scenarios
These test plans simulate realistic user behaviors against a sample Petstore web application:

*   **`scenario-petstore-catalog.jmx`**
    *   Simulates virtual users browsing the Petstore catalog, viewing different categories, and looking up items.
*   **`scenario-petstore-added_user.jmx`**
    *   Simulates the workflow of adding and registering a new user to the Petstore application, validating the data submission process.

### 3. Test Data
*   **`user_info.csv`**
    *   A CSV dataset containing user credentials and information (e.g., username, password). It is typically used in conjunction with the `CSV Data Set Config` element in the test plans to inject parameter variables into requests.

## 🚀 How to Use

1. Ensure you have **Apache JMeter (v5.5 or later)** installed on your machine.
2. Some test plans utilize external plugins (such as `Dummy Sampler` or Custom Thread Groups). Make sure to install the **JMeter Plugins Manager** and the required plugins before opening the files.
3. Open the JMeter GUI, load the desired `.jmx` file, and run the test. View the outcomes using Listeners like **View Results Tree** or **Summary Report**.

---

# JMeter 테스트 플랜

이 리포지토리는 성능 테스트, 기능 데모, 그리고 JMeter 학습을 위해 사용되는 다양한 Apache JMeter 테스트 플랜(`.jmx`) 및 관련 데이터 파일을 포함하고 있습니다.

## 📂 파일 및 시나리오

### 1. 기능 데모
이 테스트 플랜들은 JMeter 내의 특정 기능 및 컴포넌트를 시연하기 위해 설계되었습니다:

*   **`JMeter Correlation Advanced 30.jmx`**
    *   30가지의 고급 상관관계(Correlation) 연습과 다양한 **후처리기(Post-Processors/Extractors)** 예제를 포함합니다. 정규식, JSON Path, XPath, CSS Selectors 등을 사용하여 응답에서 동적 값을 정확하게 추출하는 방법을 시연합니다.
*   **`JMeter_Correlation_Examples.jmx`**
    *   동적 응답 데이터를 추출하고 이후의 요청에 활용하는 기본적인 상관관계 기법의 예제를 제공합니다.
*   **`JMeter Groovy Scripting Demo.jmx`**
    *   **JSR223 샘플러/전처리기/후처리기**와 Groovy 스크립팅을 활용하여 사용자 정의 로직, 데이터 조작 및 고급 테스트 시나리오를 구현하는 방법을 보여줍니다.
*   **`JMeter-logic-controllers.jmx`** 및 **`JMeter_Logic_Controller_sample.jmx`**
    *   JMeter의 **논리 컨트롤러(Logic Controllers)**(If, While, Switch, ForEach, Random, Throughput 등)에 대한 종합적인 데모입니다. 변수를 기반으로 테스트 실행 흐름을 동적으로 제어하는 방법을 보여줍니다.
*   **`JMeter-module.jmx`**
    *   **모듈 컨트롤러(Module Controller)**와 **테스트 프래그먼트(Test Fragments)**를 사용하여 모듈화되고 재사용 가능한 테스트 컴포넌트를 생성함으로써 복잡한 테스트 플랜의 유지보수성을 향상시키는 방법을 설명합니다.
*   **`JMeter_Thread_Group.jmx`** 및 **`threadgroup_http_example.jmx`**
    *   다양한 **스레드 그룹(Thread Groups)** 구성(예: Standard, Concurrency, Stepping)과 HTTP Request 샘플러를 통해 다양한 부하 생성 패턴을 시뮬레이션하는 방법을 보여줍니다.

### 2. Petstore 애플리케이션 시나리오
이 테스트 플랜들은 샘플 Petstore 웹 애플리케이션을 대상으로 실제 사용자의 행동을 시뮬레이션합니다:

*   **`scenario-petstore-catalog.jmx`**
    *   가상 사용자가 Petstore 카탈로그를 탐색하고, 다양한 카테고리를 확인하며, 상품을 검색하는 과정을 시뮬레이션합니다.
*   **`scenario-petstore-added_user.jmx`**
    *   Petstore 애플리케이션에 새로운 사용자를 추가 및 등록하는 워크플로우를 시뮬레이션하여 데이터 제출 과정을 검증합니다.

### 3. 테스트 데이터
*   **`user_info.csv`**
    *   사용자 자격 증명 및 정보(예: 사용자 이름, 비밀번호)가 포함된 CSV 데이터셋입니다. 주로 테스트 플랜의 `CSV Data Set Config` 요소와 함께 사용되어 요청에 파라미터 변수를 주입하는 데 사용됩니다.

## 🚀 사용 방법

1.  컴퓨터에 **Apache JMeter (v5.5 이상)** 가 설치되어 있는지 확인하세요.
2.  일부 테스트 플랜은 외부 플러그인(`Dummy Sampler` 또는 Custom Thread Groups 등)을 사용합니다. 파일을 열기 전에 **JMeter Plugins Manager**를 통해 필요한 플러그인을 설치해야 합니다.
3.  JMeter GUI를 열고 원하는 `.jmx` 파일을 로드한 후 테스트를 실행하세요. **View Results Tree** 또는 **Summary Report**와 같은 리스너(Listeners)를 사용하여 결과를 확인할 수 있습니다.
