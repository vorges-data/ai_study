### Data Preparation

1. Collection and cleaning
2. Tokenization
    - Text divided into tokens
    - Byte-Pair Encoding (BPE)
    - WordPiece

**Configuration**
1. Architecture
2. Weight Initialization

**Self-Attention**
- Allows the model to learn complex relationships between textual data
- Ensures scalability in LLMs
- Identifies essential parts of context to generate accurate responses
- Captures complex relationships in texts
- Facilitates training parallelization
- Makes training optimized, effective, and scalable

LLM training is a multidimensional process that requires attention to details such as data, architecture, and fundamental mechanisms like self-attention.

---

### Overfitting, Underfitting and Regularization

**Overfitting**
- Excessive model fitting to training data, impairing generalization by capturing noise or outliers
- Excellent performance on training and poor on validation
- High variance when evaluating new data

- Solutions:
    - Penalize model complexity (smaller weights)
        - L2 Regularization (Ridge)
        - L1 Regularization (Lasso)
        - Elastic Net

1. Dropout
    - Randomly deactivates neurons during training
    - Reduces excessive dependencies and specific combinations

2. Early Stopping
    - Stops training when validation performance starts to decline

3. Data Augmentation
    - Increases data diversity by applying transformations
        - Image rotation
        - Use of synonyms in texts

**Underfitting**
- The model does not adequately capture data relationships, having low performance on both training and validation
- High loss on training and validation
- Model with insufficient complexity for the data

- Solutions:
    - Increase model complexity
        - Add layers, neurons, or other parameters
    - Train for longer
    - Adjust hyperparameters
    - Collect more relevant data

**Regularization**
- Essential for balancing model complexity and its generalization capacity. It prevents both overfitting and underfitting
- Regularization stabilizes loss and prevents overfitting

- Dropout:
    - During training, neurons are randomly deactivated to avoid excessive dependencies
    - Effective for deep neural networks

- Weight regularization:
    - L2 Regularization (Ridge): Penalizes large weights by adding $\lambda \cdot \sum w^2$
    - L1 Regularization (Lasso): Penalizes the absolute value of weights ($(\lambda \cdot \sum |w|)$)
    - Batch Normalization: Normalizes activations in each layer, reducing the impact of poor initializations and accelerating training
    - Data Augmentation: Works as an indirect form of regularization by creating variations in input data, making the model more robust.

---

**When a model is too simple:**
- Suffers from underfitting, unable to learn relevant patterns in the data

**When a model is too complex:**
- It may suffer from overfitting, learning noise that doesn't generalize to new data

**The secret is in balance:**
- Choose the right architecture and regularization techniques so the model learns useful patterns without overdoing it.
