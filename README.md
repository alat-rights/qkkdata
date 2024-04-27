Code is slightly modified from [NanoGPT](https://github.com/karpathy/nanoGPT). (I just added hooks).

Experiment data (figures only) available in `test8`. **Experiments were run quickly. Please take data with a grain of salt.**

**SCATTERPLOTS ARE FOR REFERENCE ONLY!!** The scatterplots' scaling of the X and Y axes may not be linear. Data on the X and Y axes may have been transfored (e.g. I think the X axis is actually log).

Invocation of `sample.py` used to gather experiment data:
```
python sample.py --init_from=gpt2 --start="What is the answer to life, the universe, and everything?" --num_samples=1 --max_new_tokens=1
```

Command line output:
```
Overriding: init_from = gpt2
Overriding: start = What is the answer to life, the universe, and everything?
Overriding: num_samples = 1
Overriding: max_new_tokens = 1
loading weights from pretrained gpt: gpt2
forcing vocab_size=50257, block_size=1024, bias=True
overriding dropout rate to 0.0
number of parameters: 123.65M
No meta.pkl found, assuming GPT-2 encodings...
/usr/lib/python3/dist-packages/scipy/__init__.py:146: UserWarning: A NumPy version >=1.17.3 and <1.25.0 is required for this version of SciPy (detected version 1.25.2
  warnings.warn(f"A NumPy version >={np_minversion} and <{np_maxversion}"
Correlation: 0.07339402385562205
Correlation: 0.10989143296341713
Correlation: 0.11163160279122496
Correlation: -0.031039634080071248
Correlation: 0.08208255298725653
Correlation: 0.2322620623428199
Correlation: 0.08125741108894866
Correlation: 0.11776628531029489
Correlation: 0.13855019976307886
/usr/lib/python3/dist-packages/scipy/stats/_stats_py.py:4068: PearsonRConstantInputWarning:

An input array is constant; the correlation coefficient is not defined.

Correlation: nan
Correlation: 0.044443189287067295
Correlation: 0.13303143890458619
What is the answer to life, the universe, and everything? Have
```
