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
    
   ### Using linear activation function in output layer + (from_logits=True) -> to give flexibility in mathematical computations 

  - Fit model
    ```
    model.fit(
    X_train, y_train,
    epochs=200
    )
- Git weihts 
- Visualization of model performance
- Test training data
- Evaluate Training
- Test using unseen data
- Evaluate test

## IN training data 
 - Get true prediction for 148 of 150 example
## IN unseen data 
 - Get true prediction for 19 of 20 example
     
## Conclusion of model behavior
   you can see at layer 1 if:
      neuron 0 = 0 and neuron 1 = 0 => reault is 0
      neuron 0 = 1 and neuron 1 = 0 => reault is 1
      neuron 0 = 0 and neuron 1 = 1 => reault is 2
      neuron 0 = 1 and neuron 1 = 1 => reault is 3




























  
