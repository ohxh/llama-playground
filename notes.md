Things I've tried...


TODO

LLaMA CCS

# Setup

- Install conda
- Activate env
- Uninstall transformers
- `pip install git+https://github.com/mbehm/transformers`
- `pip install bitsandbytes-cuda117`

`AttributeError: /home/ubuntu/anaconda3/lib/python3.9/site-packages/bitsandbytes/libbitsandbytes_cpu.so: undefined symbol: cget_col_row_stats`

CD there and `cp libbitsandbytes_cuda117.so libbitsandbytes_cpu.so`!

- found error in Collin's code (returning probe instead of best_probe)