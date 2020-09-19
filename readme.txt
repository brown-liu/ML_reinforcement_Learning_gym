1.initial replay memory capacity
2.initialize the network with random weights
3.for each epsides:
	1.initialized the starting state
	2.for each time step:
		1. select and action 
			Either exploration or exploitation
		2.Execute selected auction in an emulator
		3.Observe reward and next state
		4.Store experience in replay memory
		5.Sample random batch from replay memory
		6.Preprocess states from batch
		7.Pass batch of preprocessed states to policy network
		8. Calculate loss between output Q_values and target Q-values.
			requires a second pass to the network for the next state
		9.Gradient descent updates weights in the policy network to minimize loss
