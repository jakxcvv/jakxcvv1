# Type expression agent

Is an agent that receives a reference to a mathematical expression. If the expression contains x, x^2, or x^3, it outputs the corresponding result.

---

#### **Action class: `action_translation_expression`**
Generates an equation based on a template and performs argument mapping if needed.

#### **Parameters:**
- `amountX`: The number of x in the expression

#### **Workflow:**
1. The first agent receives a reference to a mathematical expression and an input_structure. Then it translates the received expression and receives the number of X in the expression.
2. The second agent receives a structure and a translated mathematical expression and a set of rules to determine its type. Then the type is determined, for example: square and the agent produces the result.

![Example Image](https://github.com/jakxcvv/jakxcvv1/blob/main/photo_2025-04-14_10-51-00.jpg)

##**Example**

#### **Example of an input structure:**
![Example Image](https://github.com/jakxcvv/jakxcvv1/blob/main/photo_2025-04-14_10-52-11.jpg))

#### **Example of an output structure:**
![Example Image](https://github.com/jakxcvv/jakxcvv1/blob/main/photo_2025-04-14_10-52-11.jpg)

#### **Result Codes**
Possible result codes:

| Code                             | Description                                   |
|----------------------------------|-----------------------------------------------|
| `SC_RESULT_LINEAR_EQUATION`      | Linear equation                               |
| `SC_RESULT_QUADRATIC_EQUATION`   | Quadratic equation                            |
| `SC_RESULT_CUBIC_EQUATION`       | Cubic equation                                |    
