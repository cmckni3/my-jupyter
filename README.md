# My Jupyter notebooks

## Requirements

* jupyter
* zeromq 3.2 (required by jupyter for message passing)
* Ruby 2.1+ (to use Ruby kernel)
* node 0.10+ (to use JavaScript/Coffeescript kernels)
* iruby (Ruby kernel)
* jp-babel (babel kernel)

## Jupyter Setup

```bash
brew install zeromq32
pip install jupyter
```

### Install Ruby Kernel

```bash
bundle
iruby notebook # run the kernel to install it
```

### Install Node/babel

```bash
npm install
npm run babel # run the kernel to install it
```

## Running notebooks

After installing a kernel mentioned above, `jupyter notebook` will launch the
jupyter server to use notebooks.
