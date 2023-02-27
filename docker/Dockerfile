ARG IMG_TAG=1.13.0-cuda11.6-cudnn8-devel
ARG IMG_REPO=pytorch

FROM pytorch/$IMG_REPO:$IMG_TAG

RUN apt-get -y update && apt-get -y install git gcc llvm-9-dev cmake libaio-dev vim wget

RUN git clone https://github.com/smartcoop-git/2-099.git

RUN pip install git+https://github.com/smartcoop-git/2-099.git

RUN pip install pytorch-fid

WORKDIR 2-099
