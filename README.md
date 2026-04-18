# JMeter Test Plans

This repository contains various Apache JMeter test plans (`.jmx`) and related data files used for performance testing, feature demonstrations, and JMeter study.

## 📂 Files and Scenarios

### 1. Feature Demonstrations
These test plans are designed to demonstrate specific capabilities and components within JMeter:

*   **`scenario-logic-controllers.jmx`**
    *   A comprehensive demonstration of JMeter's **Logic Controllers** (If, While, Switch, ForEach, Random, Throughput, etc.). It uses `Dummy Samplers` and `JSON Extractors` to showcase how to dynamically control the test execution flow based on correlated variables.
*   **`JMeter Correlation Advanced 30.jmx`**
    *   Contains 30 advanced correlation exercises and examples of various **Post-Processors (Extractors)**. It demonstrates how to accurately extract dynamic values from responses using Regular Expressions, JSON Path, XPath, CSS Selectors, etc.
*   **`threadgroup_http_example.jmx`**
    *   Showcases different configurations of **Thread Groups** (e.g., Standard Thread Group, Concurrency Thread Group, Stepping Thread Group) and foundational HTTP Request samplers to simulate diverse load generation patterns.

### 2. Petstore Application Scenarios
These test plans simulate realistic user behaviors against a sample Petstore web application:

*   **`scenario-petstore-catalog.jmx`**
    *   Simulates virtual users browsing the Petstore catalog, viewing different categories, and looking up items.
*   **`scenario-petstore-added_user.jmx`**
    *   Simulates the workflow of adding and registering a new user to the Petstore application, validating the data submission process.

### 3. Test Data
*   **`user_info.csv`**
    *   A CSV dataset containing user credentials and information (e.g., username, password). It is typically used in conjunction with the `CSV Data Set Config` element in the Petstore test plans to inject parameter variables into requests.

## 🚀 How to Use

1. Ensure you have **Apache JMeter (v5.5 or later)** installed on your machine.
2. Some test plans utilize external plugins (such as `Dummy Sampler` or Custom Thread Groups). Make sure to install the **JMeter Plugins Manager** and the required plugins before opening the files.
3. Open the JMeter GUI, load the desired `.jmx` file, and run the test. View the outcomes using Listeners like **View Results Tree** or **Summary Report**.
