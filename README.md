# Tensorflow-playground-Neural-Network
TensorFlow Playground is an interactive tool that allows users to visualize and experiment with neural networks in real time.It's a browser-based interface where you can build simple neural networks, adjust parameters like the number of hidden layers, neurons, and activation functions, and see how these changes affect model performance.

# Input Parameters:
Epochs: 5 <br/>
Learning Rate: 0.3 <br/>
Ratio of Training to Test Data: 70% <br/>
Noise Level: 5 <br/>
Batch Size: 10 <br/>
Number of Hidden Layers: 3 <br/>
Problem Type: Classification

# Sigmoid Activation Function
<img width="1301" alt="sigmoid" src="https://github.com/user-attachments/assets/e9ced344-258e-4871-9010-943522000af8"> <br/>
Test Loss: 0.499 <br/>
Training Loss: 0.503 <br/>
→ With the Sigmoid activation function, both the training and test losses are relatively high. Sigmoid can lead to vanishing gradients, especially in deeper networks like yours with 3 hidden layers. This makes learning slow, and the model struggles to make meaningful updates to the weights, which is why the loss is high.

# ReLU Activation Function
<img width="1301" alt="relu" src="https://github.com/user-attachments/assets/c21c6326-28a1-48c1-824d-e4388fdb2597"> <br/>
Test Loss: 0.001 <br/>
Training Loss: 0.000 <br/>
→ The ReLU activation function performed exceptionally well. It effectively avoided the vanishing gradient problem and allowed the model to learn much better, resulting in almost zero training loss and very low test loss. This shows that the model generalized well and successfully minimized both losses.

# Conclusion:
→ ReLU outperformed Sigmoid in this classification task. ReLU's ability to mitigate the vanishing gradient problem allowed the model to converge much faster and with better accuracy. <br/>
→ Sigmoid, while useful for binary classification, struggled with the deeper network here, likely because of slower learning and saturation.


