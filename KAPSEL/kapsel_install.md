#### ライブラリ設定（Octa）
<p>
1. OCTA を展開（$HOME/OCTA/OCTA84）</br>
2. GOURMET/lib/linux_64/libplatform.a を libplatform_gcc.a にコピーする.
</p>

#### FFTW インストール
<p>
./configure CC=gcc CXX=g++ --prefix="XXX" CFLAGS="-O3" \ </br>
FFLAGS="-O3" --enable-openmp --enable-threads \ </br>
--enable-shared --disable-fortran </br>
make & make install
</p>
