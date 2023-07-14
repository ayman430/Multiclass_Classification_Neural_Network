# Multiclass_Classification_Neural_Network

### Definition
#### Implement Neural Network for classify 4 categories

### Tools used 
- numpy
- matplotlib
- sklearn
- tensorflow
- some ready functons to visualize model performance 

### Objectives
- Create data using make_blobs
- Visualize training data
- Create model
   - Create neural network layers
     ```
     model = Sequential(
          [
          Dense(2, activation='relu', name="L1"),
          Dense(4, activation='linear', name='L2')
          ]
      )
      ```
   - Compile model 
     ```
      model.compile(
      loss= tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
      optimizer = tf.keras.optimizers.Adam(.01)
  
       )
    
   ### Using linear activation in output layer + from_logits=True -> to give flexibility in mathematical computations 

  - Fit model
    ```
    model.fit(
    X_train, y_train,
    epochs=200
    )
     





























  
