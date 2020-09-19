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
