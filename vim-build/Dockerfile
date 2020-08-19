FROM ubuntu:18.04
RUN apt-get update 
RUN apt-get -y install build-essential 
RUN apt-get -y install libncurses5-dev git
RUN git clone --depth=1 https://github.com/vim/vim.git
WORKDIR vim/src
RUN LDFLAGS="-static" make 
