# Reward Steering with Evolutionary Heuristics for Decoding-time Alignment
DARWIN is a decode-time alignment technique that uses a reward-guided tree search framework to align the LLM and achieve comparable performance to preference optimization on 2 instruction following benchmarks.




# How to use?
To run darwin, check out the demo notebook. You can run darwin with just a few lines of code!

To run evaluation on alpaca eval benchmark, you can use the following command
```
python3 alpaca_generate.py --method='darwin'  --model_name='meta-llama/Meta-Llama-3-8B-Instruct' --range='0-805' --replacement_period=40 --iteration=3 --n_mutation=1
```
The results will be saved in a json file where the 'past_outputs' contains a list of outputs for original output and mutation cycle 1, 2, 3. Please format the output into the alpaca_eval format from https://github.com/tatsu-lab/alpaca_eval


