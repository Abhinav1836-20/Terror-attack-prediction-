# Terror-attack-prediction-
This project is about creating an interactive tool that estimates the severity level of a potential terror attack based on several risk factors. The user selects details such as the region, type of attack, weapon used, target, and number of casualties, and the system calculates a score using predefined risk values.




The project implements a rule-based classification system for predicting the severity of potential terror attacks.It is developed using Python and leverages the Gradio library to provide a web-based interactive interface.The system receives categorical and numerical inputs: region, attack type, weapon type, target type, and casualties.




Each categorical input is mapped to a numerical risk weight stored in dictionaries to quantify the contribution of that feature to overall threat.The model computes a cumulative risk score by summing the individual risk contributions of all input features.Casualty counts are incorporated as a conditional modifier that adjusts the risk score according to predefined thresholds.




The final cumulative score is evaluated using rule-based thresholds to classify the threat level into discrete categories: LOW, MEDIUM, or HIGH.The system outputs the result as a formatted string, representing the predicted severity level.The Gradio interface binds input widgets to the prediction function, ensuring real-time evaluation and response generation.




The implementation demonstrates feature engineering, where domain knowledge is encoded as numerical risk values to influence the model’s output.The architecture is modular, allowing risk weights, thresholds, and input categories to be updated independently without altering the main logic.It serves as an example of a lightweight, interpretable risk assessment model that does not require training on historical datasets.The system effectively combines user interface design, conditional logic, and rule-based scoring to provide actionable insights from structured input data.
