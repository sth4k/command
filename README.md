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
