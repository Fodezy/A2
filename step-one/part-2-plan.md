a) set batch size to 250 
b) try different epoch values (2-8)??
    - save error rates vs epoch amounts so I can graph this later. 
    - maybe create array<object>:
    [
        error_rate: float tuple --> [training, testing]
        epoch_count: int
    ]
    - can plot graphs and explain output 
c) use one hidden layer and varying amounts of hidden nodes (2 - 300)  : set epochs to 4
    - save error rates vs hidden nodes amount 
    - maybe create object: 
    [ 
        error_rate: float tuple --> [training, testing]
        hidden_node_count: int
    ]
    - can plot on graph and create tables, and explain outputs 
d) Use the two initialization methods (random and zero) 
    - save error rates vs epochs 
    - maybe choose optimal hyperparameters based on previous reports 
    - maybe create object:
    [
        error_rate: float tuple --> [training, testing]
        epoch_count: int
    ]
    - can plot and explain outputs 
e) Try different learning rates (0.0005 - 0.5) 
    - save error rates vs learning rates 
    - maybe choose optimal hyperparameters based on previous reports 
    - maybe create object:
    [
        error_rate: float tuple --> [training, testing]
        learning_rate: float
    ]
    - plot on graph and maybe table and explain results
f) Try varying hidden layers between 1-8 
    - will need to enclose the hidden layer logic within a callable method 
    - save error rate vs hidden layers 
    - maybe create object: 
    [ 
        error_rate: float tuple --> [training, testing]
        hidden_layers: int
    ]
    - plot on graph and table, explain output 
g) implement dropout method for regularization, rate between 0.2-0.5 
    - save error rate vs regularization rate
    - maybe create object: 
    [
        error_rate: float tuple --> [training, testing]
        regularization_count: double
    ]
    - plot on graph and tables and explain results 

create one overall object including all parts and hyperparameters 

object: 
[
    experiment_type: string : describes the current test (ex: "batch_size", "epoch_size")
    epochs: int : stores the number of epochs being used (ex: 1, 2, 3, ect)
    hidden_nodes: int : stores the number of nodes being used (ex [2 - 300] )
    hidden_layers: int : stores the number of hidden layers being used (ex [1 - 8] )
    learning_rate: float : stores the learning rate value being used (ex [ 0.0005 - 0.5] )
    init_mode: string : stores the initialization method being used (ex: "random", "zero")
    dropout: float --> dont think i need this 
    train_error: float : stores the training error rate found 
    test_error: float : stores the testing error rate found 
    train_error_epoch: list[float] : stores each epochs training error rate (used for plots)
    testing_error_epoch: list[float] : stores each epochs testing error rate (used for plots)

]