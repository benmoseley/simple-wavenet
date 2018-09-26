# simple-wavenet
Simple script which builds a WaveNet model using tensorflow and python

Example use:

```
# define input tensor
inputs = tf.placeholder(tf.float32, shape=(<batch_size>, <num_time_samples>, <num_input_channels>))

# define wavenet model
W = Wavenet1D(num_input_channels)
W.define_variables()

# get output tensor
outputs = W.define_graph(inputs)

# output shape = (<batch_size>, <num_time_samples>, <num_hidden_channels>)
```
