<div id="wiki-body" class="mt-4 flex-auto min-width-0 gollum-markdown-content instapaper_body">
        <div class="markdown-body>
<h4>
<a id="user-content-1-install-the-required-software" class="anchor" href="#1-install-the-required-software" aria-hidden="true"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1. Instale o software necessário</font></font></h4>
<p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">O comando a seguir instalará o Git, o CMake, um compilador e as bibliotecas usadas pelo The Forgotten Server.</font></font></p>
<p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">O Git será usado para baixar o código fonte, e o CMake será usado para gerar os arquivos de compilação.</font></font></p>
<pre><code>$ sudo apt-get install git cmake build-essential liblua5.2-dev libgmp3-dev libmysqlclient-dev libboost-system-dev libboost-iostreams-dev libpugixml-dev libcrypto++-dev
</code></pre>
<p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Substitua </font></font><code>libmysqlclient-dev</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">por </font></font><code>libmariadbclient-dev</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">no Debian 9 e acima.</font></font></p>
<h4>
<a id="user-content-2-download-the-source-code" class="anchor" href="#2-download-the-source-code" aria-hidden="true"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2. Faça o download do código fonte</font></font></h4>
<pre><code>$ git clone --recursive https://github.com/malucooo/otxserver-new.git
</code></pre>
<h4>
<a id="user-content-3-generate-the-build-files" class="anchor" href="#3-generate-the-build-files" aria-hidden="true"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">3. Gerar os arquivos de construção</font></font></h4>
<pre><code>$ cd forgottenserver<font></font>
$ mkdir build &amp;&amp; cd build<font></font>
$ cmake ..<font></font>
</code></pre>
<h4>
<a id="user-content-4-build" class="anchor" href="#4-build" aria-hidden="true"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">4. Construir</font></font></h4>
<pre><code>$ make
</code></pre>

        </div>

    </div>
