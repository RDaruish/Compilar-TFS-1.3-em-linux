# Como Compilar TFS 1.3 em linux

<b>1. Instale o software necessário</b>
   $ sudo apt-get install git cmake build-essential liblua5.2-dev libgmp3-dev libmysqlclient-dev libboost-system-dev libboost-iostreams-dev      libpugixml-dev libcrypto++-dev
   
<b>2. Faça o download do código fonte</b>
   $ git clone --recursive https://github.com/malucooo/otxserver-new.git
   
<b>3. Gerar os arquivos de construção</b>
   $ cd forgottenserver
   $ mkdir build && cd build
   $ cmake ..
 
<b>4. Construir</b>
   $ make
