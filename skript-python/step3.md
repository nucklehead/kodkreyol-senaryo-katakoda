Ann di kounya a, ou ta bezwen lè ou ekzekite skript ou a, ou bezwen li pran paramèt.

Lè mè m di paramèt la, m vle di pou li parèt konsa

`python annou-kode.py paramèt1 paramèt`

Ou ka itilize `sys.argv` pou jwenn paramèt sa yo.
<pre class="file" data-filename="annou-kode.py" data-target="replace">
import sys

print(sys.argv)
</pre>

`import` la pèmèt ou rale depandans ke python ba ou oswa ke ou enstale. `sys` se yon libreri ki ba ou aksè a detwa bagay sou sistèm ou a.

Pou ou konprann byen sa ki pral pase a, banm eksplike w kòman on pwogram ekzekite sou sistèm ou. 

Lè sistèm ou an oswa python egzekite yon pwogram, sistèm lan ba li kòm premye agiman oswa paramèt chimen fichye "path" pwogram oswa "script" la, apre sa li bay lòt agiman yo.

Ann gade poun wè

`python annou-kode.py paramèt1 paramèt`{{execute}}

ou tou wè `sys.argv` se yon list li ye.

Nou ka itilize l konsa
<pre class="file" data-filename="annou-kode.py" data-target="replace">
import sys

print(f'Jodia {sys.argv[1]}')
</pre>

`python annou-kode.py 12-06-2020`{{execute}}

Nou ka tou pwofite rale yon lòt depandans pou dat la epi fòmate l jan nou bezwen an

Nou ka itilize l konsa
<pre class="file" data-filename="annou-kode.py" data-target="replace">
import time

dat_la = time.time().format('%d%d-%m%m-%y%y%y%y')
le_a = time.time().format('%I%I:%M%M:%S%S %p')

print(f'Jodia {dat_la}')
print('Li {le_a}')
print('Mwen fini')

</pre>

`python annou-kode.py`{{execute}}
