# ClassicalHMM
An implementation of the Classical Hidden Markov model for i-order Markov chains.



### class `ClassicalHMM.HMM`:

This is the class responsible for computing the Hidden Markov model for a given list of sequences. 

#### Parameters:

- **Data** (*pandas.DataFrame*) - Dataframe with sequence data. Each row of the dataframe must contain a list of strings. The dataframe must contain 2 columns labeled `x` and `y`. The class will report an error if the length of a datapoint from `x` is not equal to length of the corresponding datapoint from `y` - 2.
- **Order** (*int, Defaults to 1*) - Number indicating the order of the markov model. 
- **Vocab_x** (*list*) - List of unique tokens in the `x` sequence.
- **Vocab_y** (*list*) - List of unique tokens in the `y` sequence.

#### Usage:

```
import HMM from ClassicalHMM
hmm = HMM(df, order, vocab_x, vocab_y)
```



#### Requirements:

- Pandas
- 



#### License:

[MIT](https://github.com/OmegAshEnr01n/ClassicalHMM/blob/main/LICENSE)
