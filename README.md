## Progressive Federated Dictionary Learning

### Abstract
This research presents an innovative method for federated learning that integrates dictionary learning approaches to tackle intra-class variation. Based on the concept of curriculum learning, we provide a gradual approach to dictionary learning that enhances the initialization of the dictionary in each local model. The process involves developing a neural network architecture using Convolutional Neural Networks in a federated learning configuration, where a curriculum is applied separately to each client. The global model combines local dictionaries by using averaging techniques, hence improving the representation of attributes throughout the full federated dataset. The experimental findings validate the effectiveness of the suggested methodology, wherein the integration of curriculum learning leads to enhanced precision. The study also compares the results obtained with and without the utilisation of dictionary and curriculum learning, demonstrating the beneficial influence on the model's performance.


### Algorithm
- Neural Network Architecture - CNN is the base model for every local client. The neural network architecture is specifically designed for image classification tasks. The model uses ReLU activations to extract features. Fully connected layers process flattened representations.
- Federated Learning - 5 client system is trained with Curriculum Learning applied independently to each client.
- Global Model which aggregates local dictionaries using averaging techniques. The convolutional layer of each local model then receives this global dictionary application, which modifies the model’s features according to the combined knowledge acquired by all clients.
