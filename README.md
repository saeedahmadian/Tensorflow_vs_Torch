# Compare Tensorflow with Pytorch using logistic regression
# Tensorflow_sv_Torch
## the followings are highlighted for the difference

torch.autograd.Variable() ==> tf.Variable()
torch.nn.function. ...    ==> tf.nn. ...
torch.nn. Seqential, Linear, Softmax ==> tf.keras.layers. Seqential, Dense, Softmax
torch.optim              ==> tf.keras.optimizers
torch.nn.Loss+ MSE, BCE and etc ==> tf.keras.losses. ...
torch.nn.Module ==> tf.keras.Model
Loss.Backward() calculated gradients ==> with tf.GradientTape() as t : Loss and t.gradient() calculated gradients
optim.step    ==> optim.applygradient(grad_var)
