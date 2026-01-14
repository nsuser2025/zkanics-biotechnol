#### src/makefile/Makefile.gfortran_mpi の編集

<p>
mpif90のバージョンによっては, -fallow-argument-mismatch が廃止されているので,
<span style="color:red;">赤文字</span>を消去する.  
</p>
<p>
&#36;(FC) -DPARALLEL -O2 -fexternal-blas <span style="color:red;">-fallow-argument-mismatch</span> &#36;(DEBUG) \ </br>
<span style="color:red;"> -fallow-argument-mismatch </span> ...
</p>

#### src/parallel.F90 の編集
