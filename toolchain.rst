
co jsem zatim pouzil za nastroje
================================

prohlizeni modelu
-----------------

na superrychle prohlednuti stl modelu staci `openscad <http://www.openscad.org/>`_,
staci vytvorit soubor s obashem::

  import_stl("1mmSquare.stl");

ten otevrit v openscadu a F5 vyrenderuje model.

priklady stl modelu:

  * http://www.thingiverse.com/thing:3540 (kalibracni ctverecek)
  * http://github.com/josefprusa/PrusaMendel (master branch je nase tiskarna)

rozrezani
---------

`slic3r <http://slic3r.org/>`_ se pri prvni spusteni nastavi - staci vyplnit defaulty,
jak radi pruvodce. Pak uz jen::

  File>Quick Slice..

a v adresari kde je stl soubor se vytvori gcode soubor.

kvbikuv `nejposlednejsi configurak <https://github.com/kvbik/bordel/blob/master/reprap/slic3r.black.ini>`_.

ovladani tiskarny
-----------------

``pronterface.py`` z `Printrun <https://github.com/kliment/Printrun>`_ baliku umi nasucho hybat motorkama,
extrudovat a zahrivat desku a hotend, ale taky naloadovat gcode soubor a pustit tisk.

firmware
--------

v arduinu je nahrany `Sprinter <https://github.com/kliment/Sprinter>`_ z branche experimental.
do adresare ``sprinter`` jsem nahral nase konfiguraky, konkretne pasuji na revizi ``1f11008dc856d50c730f09e63dae1d69daba6e6f``.

kompilovano je to v ``arduinu 0023``, i kdyz uz snad podporuji (alespon castecne) ``1.0``.

