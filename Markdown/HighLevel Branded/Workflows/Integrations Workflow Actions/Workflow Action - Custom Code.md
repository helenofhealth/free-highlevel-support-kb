**Date Updated:** 2024-09-08T23:55:20.000Z

**TABLE OF CONTENTS**

* [Overview](#Overview)
* [Action Name](#Action-Name)
* [Action Description](#Action-Description)
* [Action Details](#Action-Details)
* [Example](#Example)

##   

## Overview

The **Custom Code** action allows you to extend your workflow’s functionality by writing and executing custom JavaScript code. You can include properties from previous steps, perform operations, and return the output to be used in subsequent steps.

### 

  
## Action Name

**Custom Code**

  
## Action Description

The **Custom Code** action enables the execution of JavaScript code within a workflow, allowing users to extend the system’s functionality. This action can process data and return output that can be used in the workflow’s subsequent steps.

  
## Action Details

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032467316/original/J_XDJ_paKZxPI-1e39hRdh68vOEr0s-dbQ.png?1725819732)

  
### **How to Configure**

1. **Action Name:** Give your custom code step a name that reflects its purpose.
2. **Language:** By default, this is set to JavaScript. Currently, no other languages are supported.
3. **Property to Include in Code:**  
   * Add key-value pairs where the key will be used in your code, and the value can either be hardcoded or dynamically mapped from previous workflow steps.  
   * Use these key-value pairs within the code by referencing `inputData.<key>`. For example, if the key is `number1`, you can access it in the code as `inputData.number1`.
4. **Code:**  
   * Write JavaScript code to process the values mapped in the previous step.  
   * Ensure the output is in the form of a JavaScript object or array of objects. Example: `output = { result: sum }`.
  
  
| Field Name                  | Description                                                                                                                | Mandatory |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------- | --------- |
| Action Name                 | The name of the action that will be displayed in the workflow.                                                             | Yes       |
| Language                    | The programming language used for the custom code (default is JavaScript).                                                 | Yes       |
| Property To Include In Code | Fields to be used within the code, mapped from previous steps. Use inputData.keyName to access the values within the code. | Yes       |
| Code                        | JavaScript code to perform the desired operation. The output should be a JavaScript object.                                | Yes       |

##   

## Example

javascript

Copy code

`// This is wrapped in an async function
const sum = inputData.number1 + inputData.number2;

// Return the result as a JavaScript object
output = { result: sum };
`

This example adds two numbers from the mapped properties `number1` and `number2` and outputs their sum.