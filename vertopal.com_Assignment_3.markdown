---
jupyter:
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.11.10
  nbformat: 4
  nbformat_minor: 5
---

::: {#8a98da66-3bfe-4366-ae31-38ae273d9bf7 .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"raw\",\"checksum\":\"d69bf099127822d98626842a6ae0b687\",\"grade\":false,\"grade_id\":\"cell-b97333c5a681a571\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
This material, no matter whether in printed or electronic form, may be
used for personal and non-commercial educational use only.\
Any reproduction of this manuscript, no matter whether as a whole or in
parts, no matter whether in printed or in electronic form, requires
explicit prior acceptance of the authors.
:::

::: {#649a1df7-3a9c-4cef-82f0-b10815d13781 .cell .markdown revert="_version 1.1_"}
*version 1.1*
:::

::: {#9cb77e9f-a55a-47e5-a948-a09a7f0d207a .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"markdown\",\"checksum\":\"f4117093b184911f657f98aef9656e59\",\"grade\":false,\"grade_id\":\"cell-399732cc128cd1fd\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
`<br>`{=html}`<br>`{=html}
`<span style="font-size:2em;font-weight:lighter;">`{=html}194.025
Introduction to Machine Learning`</span>`{=html}`<br>`{=html}
`<span style="font-size:3em;font-weight:normal;line-height:70%;">`{=html}Assignment
3: Regression & Gradient Descent`</span>`{=html}

------------------------------------------------------------------------
:::

::: {#05df28b7-fecb-4108-a0a5-846004387039 .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"markdown\",\"checksum\":\"fa1baeff1e027e98db832eb143920182\",\"grade\":false,\"grade_id\":\"cell-e554d74df24910b6\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
Welcome to the third assignment of our course **Introduction to Machine
Learning**. You will be able to earn up to a total of 10 points. Please
read all descriptions carefully to get a full picture of what you have
to do.

**Remark:** Some code cells are put to read-only. Please execute them
regardless as they contain important code. You can run a jupyter cell by
pressing `SHIFT + ENTER`, or by pressing the play button on top (in the
row where you can find the save button). Cells where you have to
implement code contain the comment `# YOUR CODE HERE` followed by
`raise NotImplementedError`. Simply remove the
`raise NotImplementedError`and insert your code.

Some other code cells start with the comment `# hidden tests ...`.
Please do not change them in any way as they are used to grade the tasks
after your submission.
:::

::: {#46ea9b17-9a18-48a4-8573-4b869a2a5fe6 .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"markdown\",\"checksum\":\"d8168b76d40575adb6b216116c1499e3\",\"grade\":false,\"grade_id\":\"cell-31a5613a82d15456\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
## Implement Gradient Descent for Linear Regression (4 Points)

Implement the algorithm on the slide titled \'Gradient Descent\' of the
\'Basic Algorithms I\' slides.

Ensure that you implement the algorithm using exactly the interface
described below.

`def gradient_descent_linear_regression(X, y, initial_w, learning_rate, epochs)`

#### Note:

-   To be on the safe side with our auto grading tool, please do not
    start your names for variables, functions, etc. with `solution_`
-   Be careful about integer/ float division in python
:::

::: {#bf8c4437-c45b-4d94-9e21-b99e9e9776c5 .cell .code execution_count="1" deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"8eba43eebc8f46d96e75033aaa168e08\",\"grade\":false,\"grade_id\":\"cell-02482c892faa987e\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
import numpy as np
import numpy.linalg as la
import matplotlib.pyplot as plt
```
:::

::: {#6a35cfea-fa03-4917-b30f-ee93face451e .cell .code execution_count="2" deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"4217abc34ec46913e99da3e83cb8b3ca\",\"grade\":false,\"grade_id\":\"cell-9b5150f5408a6e71\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# a data sample without noise to toy around, you may use different data

X = np.linspace(10, 20, 50)
y = 2.5 * X + 4.0
```
:::

::: {#e2b1d8ac-34f4-426e-bd0e-203ee8532699 .cell .code deletable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"34e688d3ef1edb639b581307da41b57e\",\"grade\":false,\"grade_id\":\"cell-851aa3bea2ca6756\",\"locked\":false,\"schema_version\":3,\"solution\":true,\"task\":false}" revert="def gradient_descent_linear_regression(X, y, initial_w, learning_rate, epochs):
    '''
    X: 1d numpy array containing floats
    y: 1d numpy array containing floats
    initial_w: 1d numpy array containing exactly two float values [w_0, w_1]
               that are used to initialize w_0 and w_1
    learning_rate: float
    epochs: int

    expected output: 1d numpy array containing exactly two float values [w_0, w_1]
    '''
    # YOUR CODE HERE
    raise NotImplementedError()"}
``` python
def gradient_descent_linear_regression(X, y, initial_w, learning_rate, epochs):
    '''
    X: 1d numpy array containing floats
    y: 1d numpy array containing floats
    initial_w: 1d numpy array containing exactly two float values [w_0, w_1]
               that are used to initialize w_0 and w_1
    learning_rate: float
    epochs: int

    expected output: 1d numpy array containing exactly two float values [w_0, w_1]
    '''
    # YOUR CODE HERE
    raise NotImplementedError()
```
:::

::: {#cff734b7-8f19-47f7-8934-cd7573f44945 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"7a9420062c254fc5fd4c9a2a39b8da46\",\"grade\":true,\"grade_id\":\"cell-f67f571c9d87ab9d\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#b500f9b7-47c2-4c27-8152-4d96c98e60cb .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"dd1dc704a0dbfd4d9e2e2b983a8c60b2\",\"grade\":true,\"grade_id\":\"cell-58f768f15158808c\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#49630fd6-71e2-486f-a731-5e5af6793e47 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"fef3d8e9d053d0e394a8ff724b5a460e\",\"grade\":true,\"grade_id\":\"cell-fc503dbebe61dcdf\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#4f7e7818-fd2d-4ecb-ae6b-1a7aae59be64 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"8fbd80f93ae6ca07231469689b220a36\",\"grade\":true,\"grade_id\":\"cell-bd8758c0a39d1a88\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#9388c5e8-81a3-4292-86ef-0183e2459d41 .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"markdown\",\"checksum\":\"20f4a3b4bf4d88f769dd1debc298d14a\",\"grade\":false,\"grade_id\":\"cell-b71c55f299bf3ed6\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
## Comparison to Closed Form Linear Regression (2 Points)

Luckily, we know that we can compute $w_1$ and $w_0$ (more or less)
exactly using the \'Closed Form Solution\' equalities.

Implement \'Some Python Code\' to compute $w_1$ and $w_0$ for the data
set given in the next cell.

Fix the learning rate for your gradient descent algorithm to
`learning_rate=0.000001`

How many epochs do you need to get the parameters right up to an error
of `0.1` when starting at `initial_w=np.array([2,12])`?

Assign your answer to the variable `reply_number_of_epochs`

Is this surprising to you?

**Hint 1:** You can check if all values of two arrays `a` and `b` are at
least x apart with

    np.allclose(a,b, atol=x, rtol=0)

**Hint 2:** Looping over all values might not be the fastest solution.
:::

::: {#3c62cece-2916-46a6-86b0-01e1d05b2b65 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"6ac586546fdc46bb59a33057e83f9571\",\"grade\":false,\"grade_id\":\"cell-502dfb4d53750156\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
X2 = np.array([-1., -0.95918367, -0.91836735, -0.87755102, -0.83673469, -0.79591837, -0.75510204, -0.71428571, -0.67346939, -0.63265306, -0.59183673, -0.55102041, -0.51020408, -0.46938776, -0.42857143, -0.3877551, -0.34693878, -0.30612245, -0.26530612, -0.2244898, -0.18367347, -0.14285714, -0.10204082, -0.06122449, -0.02040816, 0.02040816, 0.06122449, 0.10204082, 0.14285714, 0.18367347, 0.2244898, 0.26530612, 0.30612245, 0.34693878, 0.3877551, 0.42857143, 0.46938776, 0.51020408, 0.55102041, 0.59183673, 0.63265306, 0.67346939, 0.71428571, 0.75510204, 0.79591837, 0.83673469, 0.87755102, 0.91836735, 0.95918367, 1.])
y2 = np.array([-16.01888673, -15.06215775, -14.66563224, -13.98386833, -13.15288414 , -12.33027782, -11.92996315, -10.80118307, -10.51458662, -9.65801659 , -9.00459352, -8.46469268, -7.25778365, -6.50155011, -6.38382577 , -5.69013565, -5.07691771, -4.64218747, -3.56640217, -2.53184116 , -2.01569423, -1.09869641, -0.87069945, 0.71259073, 0.90882325 , 1.37826874, 2.23373936, 2.81463612, 4.03562475, 3.63696536 , 4.13601676, 5.68708623, 6.04695401, 7.2627373, 7.74624043 , 8.78626548, 8.50347204, 10.48395259, 9.86322328, 10.84944206 , 11.58472135, 12.46780085, 13.21365486, 13.7756522, 14.59631027 , 15.84471266, 15.82315378, 16.15334549, 17.36419808, 17.79100676])
```
:::

::: {#47ca32f6-e712-4115-a5ab-ae545d55ea52 .cell .code deletable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"47b20b8ae0f27383f2134c4c3625a06a\",\"grade\":false,\"grade_id\":\"cell-05b0b59ae719d398\",\"locked\":false,\"schema_version\":3,\"solution\":true,\"task\":false}" revert="reply_number_of_epochs = 1  # this is certainly not enough ;)

# overwrite the variable (use the same name) with a value of your choice)

# YOUR CODE HERE
raise NotImplementedError()"}
``` python
reply_number_of_epochs = 1  # this is certainly not enough ;)

# overwrite the variable (use the same name) with a value of your choice)

# YOUR CODE HERE
raise NotImplementedError()
```
:::

::: {#d139b774-837d-43f3-8824-180e201bc917 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"4e9119d88b41b1af4dca49801e7e3fbe\",\"grade\":true,\"grade_id\":\"cell-49f4faac90192701\",\"locked\":true,\"points\":2,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#e2577dd3-3211-4321-ba58-a6ccbc6285b9 .cell .markdown deletable="false" editable="false" nbgrader="{\"cell_type\":\"markdown\",\"checksum\":\"cabf054872e962f4bc889233adb93f22\",\"grade\":false,\"grade_id\":\"cell-2d2ddc7a8b55e94b\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
## Polynomial Regression (4 Points)

Implement polynomial regression for one-dimensional input, but arbitrary
degree, as described on the slide \'What About Polynomial Regression,
then?!?\'. That is, the user of your method should be able to specify
the degree of the polynomial to fit as a parameter. Note that a
polynomial of degree $p$ has $p+1$ entries in the vector $\mathbf{w}$.
The polynomial should look as follows:

$$h(x) = \sum_{k=0}^p w_k \cdot x^k\;.$$

Also implement the function that, given a weight array
`np.array([w_0, w_1, ..., w_p])` can compute the function values of the
corresponding polynomial.

Ensure that you implement the algorithm using exactly the interface
described below.
:::

::: {#fc313277-12ef-4d64-8eae-411a9de482cf .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"8d2702f3d872d85c3451df5beeee3482\",\"grade\":false,\"grade_id\":\"cell-ce6cf667773fcf32\",\"locked\":true,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
import numpy as np
import numpy.linalg as la
```
:::

::: {#75fe46ad-6bcb-4cae-b3bf-d7db3389c18d .cell .code deletable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"accdb0712c658b6655ea34d14a88cd3f\",\"grade\":false,\"grade_id\":\"cell-6e12a2ea6441deae\",\"locked\":false,\"schema_version\":3,\"solution\":true,\"task\":false}" revert="def poly_regression_fit(X, y, p):
    '''
    X: 1d numpy array containing floats
    y: 1d numpy array containing floats
    p: a nonnegative integer, giving the degree of the polynomial

    expected output: 1d numpy array containing the float values [w_0, w_1, ..., w_p]
    '''
    # YOUR CODE HERE
    raise NotImplementedError()"}
``` python
def poly_regression_fit(X, y, p):
    '''
    X: 1d numpy array containing floats
    y: 1d numpy array containing floats
    p: a nonnegative integer, giving the degree of the polynomial

    expected output: 1d numpy array containing the float values [w_0, w_1, ..., w_p]
    '''
    # YOUR CODE HERE
    raise NotImplementedError()
```
:::

::: {#96f01e75-043c-41e4-b586-a13c2336e0f0 .cell .code deletable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"ae662f0b962c3dd50f2b6e2e36c376e1\",\"grade\":false,\"grade_id\":\"cell-7901645cc3379eb6\",\"locked\":false,\"schema_version\":3,\"solution\":true,\"task\":false}" revert="def poly_regression_transform(X, w):
    '''
    X: 1d numpy array containing floats
    w: 1d numpy array containing the float values [w_0, w_1, ..., w_p]

    expected output: 1d numpy array, same shape as X, containing function values
    '''
    # YOUR CODE HERE
    raise NotImplementedError()"}
``` python
def poly_regression_transform(X, w):
    '''
    X: 1d numpy array containing floats
    w: 1d numpy array containing the float values [w_0, w_1, ..., w_p]

    expected output: 1d numpy array, same shape as X, containing function values
    '''
    # YOUR CODE HERE
    raise NotImplementedError()
```
:::

::: {#7f6208fd-ddb9-4e77-a38c-000c7d8d8344 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"c0101368fadeac98989c5a4f2ce66491\",\"grade\":true,\"grade_id\":\"cell-178eec931c20b7af\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#2d72bbdc-6bbc-4120-a266-9d2292221e5f .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"d0ce5289eae30f519456da3f36180d6f\",\"grade\":true,\"grade_id\":\"cell-aa2ff8382a25f60f\",\"locked\":true,\"points\":1,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::

::: {#46ca9803-e177-4d91-a201-e28b08d94867 .cell .code deletable="false" editable="false" nbgrader="{\"cell_type\":\"code\",\"checksum\":\"44d52fe75d8fb496863bc7888c5fa5f4\",\"grade\":true,\"grade_id\":\"cell-d0f05153a90aa63b\",\"locked\":true,\"points\":2,\"schema_version\":3,\"solution\":false,\"task\":false}"}
``` python
# hidden tests - DO NOT CHANGE THIS CELL
```
:::
