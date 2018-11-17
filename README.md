# Como Compilar TFS 1.3 em linux
<br>
<br>
<b>1. Instale o software necessário</b><br>
   $ sudo apt-get install git cmake build-essential liblua5.2-dev libgmp3-dev libmysqlclient-dev libboost-system-dev libboost-iostreams-dev      libpugixml-dev libcrypto++-dev
<br>

<b>2. Faça o download do código fonte</b><br>
   $ git clone --recursive https://github.com/malucooo/otxserver-new.git
<br>

<b>3. Gerar os arquivos de construção</b><br>
   $ cd forgottenserver
   $ mkdir build && cd build
   $ cmake ..
 <br>
 
<b>4. Construir</b><br>
   $ make
