Ann di ou renmen script ou fè a e ou ta renmen pataje l.

Li t ap enpòtan pou dokimante paramèt yo.

Eben ou ka mete dokimantasyon an nan skript la menm!

Pou sa, n'ap itilize `argparse`

<pre class="file" data-filename="annou-kode.py" data-target="replace">
import argparse

parser = argparse.ArgumentParser(description='Pwogram pou ekri dat ak lè')

parser.add_argument('--dat_la', help='Dat ou bezwen m ba ou a')
parser.add_argument('--le_a', help='Lè ou bezwen m ba ou a')

</pre>

Nou itilize `ArgumentParser` pou kreye zouti ki ap jere sa pou nou an.

Fonkson oswa metòd `add_argument` la ajoute enfòmasyon pou paramèt yo


<pre class="file" data-filename="annou-kode.py" data-target="append">
agiman = parser.parse_args()

dat_la = agiman.dat_la
le_a = agiman.le_a

print(f'Jodia {dat_la}')
print('Li {le_a}')
print('Mwen fini')
</pre>

Lè ou fè `parse_args()` ou di l pou li ranmase agiman yo epi mete enfòmasyon an nan varya `agiman` an.

Kounya a si ou pa itilize ankeen agiman, ou wè li ap ba w detay yo pou ka byen itilize script la.

`python annou-kode.py`{{execute}}

Ann tests ak bon paramèt yo.

`python annou-kode.py --dat_la 12-06-2020 --le_a "2:40:10 PM"`{{execute}}
