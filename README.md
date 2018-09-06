# command
command to install virtualenv, cuda, cudnn, etc


# install Virtualenv

$pip install virtualenv

$pip install virtualenvwrapper

$mkdir ~/.virtualenvs

#add to ~/.bashrc

export WORKON_HOME=~/.virtualenvs

source ~/.local/bin/virtualenvwrapper.sh

$source .bashrc

$mkvirtualenv my-virtual-environment --system-site-packages target-directory

$workon my-virtual-environment

# install cuda
https://gist.github.com/zhanwenchen/e520767a409325d9961072f666815bb8#install-cuda


# install cudnn
tar xvf cudnn*.tgz

cd cuda

sudo cp */*.h /usr/local/cuda/include/

sudo cp */libcudnn* /usr/local/cuda/lib64/

sudo chmod a+r /usr/local/cuda/lib64/libcudnn*

# install tensorflow-gpu, make sure the version is compatible with cuda

pip install tensorflow-gpu==1.4.1



# Install Jupiter notebook

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-jupyter-notebook-to-run-ipython-on-ubuntu-16-04


# RE

## chinese characters and punctuations

`re.compile(u'[\u4E00-\u9FA5|\u3002|\uff1f|\uff01|\uff0c|\u3001|\uff1b|\uff1a|\u201c|\u201d|\u2018|\u2019|\uff08|\uff09|\u300a|\u300b|\u3008|\u3009|\u3010|\u3011|\u300e|\u300f|\u300c|\u300d|\ufe43|\ufe44|\u3014|\u3015|\u2026|\u2014|\uff5e|\ufe4f|\uffe5]')`

## English Chacters and punctuations

`re.compile(u'[\x00-\x80]+')`
