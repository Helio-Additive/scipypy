# Scipypy

Scipypy is an unofficial mirror of the code version of Pypy that perfectly runs the Python scientific packages like Numpy, Scipy, and Pandas. Pypy native support for such packages has been an effort largely achieved since pypy3.7, but sometimes things don't work as expected. 

This repo hosts the latest versions of Pypy that will run scientific stack just fine, most importantly without needing conda. Pip install should suffice.


## Installation

```bash
wget https://github.com/Helio-Additive/scipypy/releases/download/latest/latest-linux64.tar.gz
#OR
curl -LJO https://github.com/Helio-Additive/scipypy/releases/download/latest/latest-linux64.tar.gz

#Installation on Linux
tar -xzvf latest-linux.tar.gz pypy/

#Soft symbolic link needs full path else won't work (dangling operations)
ln -s /home/..../path/to/the/expanded-archive/pypy/bin/pypy3.9 /usr/local/bin/pypy

sudo chmod ugo+x /usr/local/bin/pypy

#Enjoy
pypy -m pip install numpy

```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
