![university logo](Logo_HSCoburg_ENG_RGB_Rot.svg)
# 1 Car Speed Tracking in a Video

**Difficulty:** Easy | **Type:** L&L

We have developed a program that tracks a car in a video (a sequence of frames) and measures its speed. We have already recorded measurements for a duration of 10 seconds. A sample of the recorded data is:

- $D1 (1, 6)$
- $D2 (9, 22)$

The first element represents time (in seconds), and the second element represents speed (in kilometers per hour). Our manager expects us to determine a model describing the car's speed over time. She specifically expects a linear equation of the form:

$$
y = a \cdot x + b
$$

## To-Dos
1. **Visualize the Data**  
   - Plot the given data points using a tool like `GeoGebra`, `Matplotlib`, or on paper.
   - Set up a coordinate system with time on the $x$-axis and speed on the $y$-axis.

2. **Formulate the Equation System**  
   - Insert the given data points into the linear equation.

3. **Convert to Matrix Form**  
   - Express the system as a matrix equation.
   - Determine whether the matrix is invertible and justify your answer.
   - Identify and name the components of the equation in matrix form.

4. **Solve for $a$ and $b$**  
   - Solve the system manually.
   - Use computational tools like `linalg.inv` to compute the inverse matrix if necessary.

5. **Verify with Computational Tools**  
   - Solve the system using `linalg.solve` or another tool.
   - Compare the computed results with your manual calculations.

6. **Plot the Linear Function**  
   - Visualize the computed line.
   - Predict the car's speed at $t = 20s$ using the model.


# 2 Car Speed Tracking with Additional Data  

**Difficulty:** Easy | **Type:** D&L     

To challenge us further (and improve our model), our manager has provided two additional measurements. The updated dataset is:  

- $D1 (1, 6)$  
- $D2 (3, 18)$  
- $D3 (7, 14)$  
- $D4 (9, 22)$  

As before, the first element represents time (in seconds), and the second element represents speed (in kilometers per hour). Our manager still expects us to determine a model describing the car's speed over time, again assuming a linear equation:  

$$
y = a \cdot x + b
$$  

## To-Dos  

1. **Visualize the Data**  
   - Plot the given data points as in the first task.  
   - Use tools like `GeoGebra`, `Matplotlib`, or paper.  

2. **Formulate the Equation System**  
   - Set up the system of equations using the given data points.  

3. **Convert to Matrix Form**  
   - Express the system as a matrix equation.  
   - Determine whether the matrix is invertible and justify your answer.  
   - Identify and name the components of the equation in matrix form (this time independently).  

4. **Solve for $a$ and $b$**  
   - Solve the system manually.  
   - Compute the **pseudoinverse** using tools like `linalg.pinv`.  
   - Before using `linalg.pinv`, attempt to calculate the pseudoinverse manually (use tools for matrix multiplication if needed).  

5. **Verify with Computational Tools**  
   - Solve the system using `linalg.lstsq` or another tool.  
   - Compare the computed results with your manual calculations.  

6. **Plot the Linear Function**  
   - Visualize the computed line.  
   - Predict the car's speed at $t = 20s$ using the model.  

# 3 Car Speed Tracking with a Parabolic Model  

**Difficulty:** Medium | **Type:** D&L 

Our manager has changed her mind. Instead of a linear model, she now wants a **parabolic model** to describe the car's speed:  

$$
y = a x^2 + b x + c
$$  

Additionally, our program was applied to another car in a different video, producing the following measurements:  

- $D1 (1, 12.8)$  
- $D2 (5, 23.5)$  
- $D3 (7, 21.3)$  
- $D4 (10, 22.2)$  

## To-Dos  

1. **Visualize the Data**  
   - Plot the given data points as in previous tasks.  
   - Use tools like `GeoGebra`, `Matplotlib`, or `paper`.  

2. **Formulate the Equation System**  
   - Set up the system of equations using the given data points and the quadratic model.  

3. **Convert to Matrix Form**  
   - Express the system as a matrix equation.  
   - Determine whether the matrix is invertible and justify your answer.  
   - Identify and name the components of the equation in matrix form.  

4. **Solve for $a$, $b$, and $c$**  
   - Solve the system manually.  
   - Compute the **(pseudo)-inverse** using tools like `linalg.pinv`.  

5. **Verify with Computational Tools**  
   - Solve the system using `linalg.lstsq` or another tool.  
   - Compare the computed results with your manual calculations.  

6. **Plot the Parabolic Function**  
   - Visualize the computed parabola.  
   - Predict the car's speed at $t = 20s$ using the model.  



# 4 Face Completion with Linear Regression  

**Difficulty:** Medium | **Type:** C&L

Our manager has given us a new challenge: **face completion using linear regression**. She wants us to investigate how **linear regression** can be used to reconstruct missing parts of an image.  

For this experiment, we will work with **grayscale images of faces**. However, part of the image has been **lost**, leaving a blank section. Our task is to use a **linear regression estimator** to predict the missing pixels based on the surrounding ones.  

## To-Dos  

1. **Visualize the Data**  
   - Load the given dataset and display it.  

2. **Prepare the Training Data**  
   - Separate the available pixel values into **features (X)** and **targets (y)**.  
   - Define which part of the image will be used for training and which part will be predicted.  

3. **Train a Linear Regression Model**  
   - Use **scikit-learn's LinearRegression** to train a model on the known pixel values.  
   - Fit the model using the available data and prepare it to predict the missing pixels.  

4. **Predict the Missing Pixels**  
   - Use the trained model to estimate the values of the missing pixels.  
   - Reconstruct the image by filling in the blank section with the predicted values.  

5. **Display and Compare the Results**  
   - Show the **original image**, the **image with missing pixels**, and the **reconstructed image**.  
   - Evaluate the quality of the reconstruction: Does the completed section blend well with the rest of the image?  

6. **Discussion**  
   - What are the strengths and weaknesses of using **linear regression** for image completion?  
   - How could a more advanced model (e.g., neural networks) improve the results?  


# 5 Kaggle Python Course

**Difficulty:** Easy | **Type:** O

Kaggle ([https://www.kaggle.com/](https://www.kaggle.com/)) offers several short courses that include **practical examples and exercises**. These courses are in **English** and provide a **certificate** upon completion, which can be useful for future applications.  

## To-Do  

Try to complete the **Kaggle Python Course**:  

[https://www.kaggle.com/learn/python](https://www.kaggle.com/learn/python)  
