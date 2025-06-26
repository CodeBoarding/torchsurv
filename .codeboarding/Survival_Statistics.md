```mermaid
graph LR
    KaplanMeierEstimator["KaplanMeierEstimator"]
    IPCWCalculator["IPCWCalculator"]
    InputValidator["InputValidator"]
    IPCWCalculator -- "uses" --> KaplanMeierEstimator
    KaplanMeierEstimator -- "uses" --> InputValidator
    IPCWCalculator -- "uses" --> InputValidator
    click KaplanMeierEstimator href "KaplanMeierEstimator.html" "Details"
    click IPCWCalculator href "IPCWCalculator.html" "Details"
    click InputValidator href "InputValidator.html" "Details"
```

[![CodeBoarding](https://img.shields.io/badge/Generated%20by-CodeBoarding-9cf?style=flat-square)](https://github.com/CodeBoarding/GeneratedOnBoardings)[![Demo](https://img.shields.io/badge/Try%20our-Demo-blue?style=flat-square)](https://www.codeboarding.org/demo)[![Contact](https://img.shields.io/badge/Contact%20us%20-%20contact@codeboarding.org-lightgrey?style=flat-square)](mailto:contact@codeboarding.org)

## Details

Overview of the core components within the `Survival Statistics` subsystem of `torchsurv`, outlining their structure, purpose, and interactions. These components are fundamental for performing key statistical analyses in survival modeling.

### KaplanMeierEstimator [[Expand]](./KaplanMeierEstimator.md)
This component is responsible for computing the Kaplan-Meier survival estimates. It takes event and time data as input and provides methods to calculate survival probabilities over time, including the option to estimate the censoring distribution. It also offers utility methods for plotting and predicting estimates on new time points.


**Related Classes/Methods**:

- `KaplanMeierEstimator` (1:1)


### IPCWCalculator [[Expand]](./IPCWCalculator.md)
This component is responsible for calculating Inverse Probability of Censoring Weights (IPCW). It leverages the `KaplanMeierEstimator` to model the censoring distribution and then computes the inverse probabilities, which are crucial for unbiased estimation in the presence of censored data.


**Related Classes/Methods**:

- `IPCWCalculator` (1:1)


### InputValidator [[Expand]](./InputValidator.md)
This utility component provides functions to validate the format, types, and integrity of survival data inputs (e.g., event and time tensors) used across various functions and classes within the `torchsurv` subsystem. It ensures data quality and prevents common errors.


**Related Classes/Methods**:

- `InputValidator` (1:1)




### [FAQ](https://github.com/CodeBoarding/GeneratedOnBoardings/tree/main?tab=readme-ov-file#faq)