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
brew install zmq
pip install virtualenv virtualenvwrapper
source /usr/local/bin/virtualenvwrapper.sh
mkvirtualenv jupyter
pip install -r requirements.txt
```

See [virtualenvwrapper](http://virtualenvwrapper.readthedocs.io/en/latest/) for more information

### Install Ruby Kernel

Install Ruby 2.1 or higher using your favorite method. I prefer [rbenv](https://github.com/rbenv/rbenv#installation)

```bash
bundle
bundle exec iruby notebook # run the kernel to install it
```

### Install Node/babel

Install node.js 0.10 or higher using your favorite method. I prefer [nvm](https://github.com/creationix/nvm#installation)

```bash
yarn install
yarn babel # run the kernel to install it
```

## Running notebooks

After installing a kernel mentioned above, `jupyter notebook` will launch the
jupyter server to use notebooks.
