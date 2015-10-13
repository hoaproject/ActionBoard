APEX 3
======

Conf Pierre Joye `PHP 7 HHVM & co` :

Give feedback to pierrejoye about php5.6 >= by twitter.


PICKLE
======

Installation extension PHP comme les PEAR PHP
PEAR sera abandonné dans l'avenir

Creation d'un system de package comme sur packageist.

RFC PHP > 7
===========

Permet aux dev de documenter leur proposition d'implementation.

RFC Release process :

listing des versions feature supporter pour chaque version de PHP à partir de 5.4
avec un cycle de vie de 3ans.

2 premières année sont en upstream avec des bugfix.

NO BC Break entre chaque sous version 5.5 > 5.6 > 5.7
5.4 is dead, go to 5.6

5.5 is only security fix, because it's last year.

RC toutes les 2 semaines sur 5.6 & 7
Last stable version is 5.6.13

PHP 7.0.0 RC3 sorti mi septembre 2015.

BENCHMARK
=========

Beaucoup de benchmark par des grands acteur facebook & co
fight vs HHVM & PHP7

les deux sont proche, beaucoup de faux benchmark.

test php7 et deployer le sur des prod et report him.


Wordpress 4.1.1 : PHP6 et HHVM same perf result (2 fois plus rapide avec php7 que php5)


FEATURES PHP7
=======

Rewamped Engine
true 64bit support
Large string and LFS
Consistent variables syntax
Error exception on fatal error
Scalar type declarations
Zero cost asserts

Secure RNG (Génération de nombre aléatoire sécurisé, true random)
PHP4 Constructors deprecated
JIT enabled PCRE
Removed ext/mysql, ext/ereg and more
New ?? and spaceship operators
New JSON parser

Look at RFC for target to 7.1


Scalar TYPE Declaration
========

use delcare strict pour forcer l'appel et la déclaration de type stricte

Null Coalesce opertor
=======

$x ?? $y ?? $z

php-langspec
======

https://github.com/php/php-langspec

Open & Public spec


QB Compiler
======

permet de re definir ses propre type de variable l'interieur d'une fonction
qui embarque un moteur virtuel.

avec le mode JIT ce sera compiler en mode natif à la volé.

http://php-qb.net/index.php/2-uncategorised/27-comparing-performance-in-qb-with-hhvm


QB implement que le code interne de la fonction en natif et non ses appels.


Zephir
======

Cree une fonction php et la compile avec Zephir en lib system.
et l'implement dans php a chaud.


PHP Alternative implementations
=====

HHVM (native code)
Recki-ct (native code) ircMaxWell
Phalanger (.net engine)

Recki-ct permet de généré un code pre compiler qui sera executer en JIT avant de partir sur du native code.

benchphp dans les sources github


2 EM JOURS =>>>
===============



MAIL SYSTEM
===========

Résumé des recherches sur des services mail associatifs

SMTP
IMAP
MAIL LIST

SERVER
======

Prise de décision si on prend une machine sur Azure ou Microsoft avant fin novembre.

Demande à CARLOS et comparaison de tarif pour AWS


RETROPSPEC
==========

Important retro :

    * Contribution :

        * Frustration
        * Present sur IRC ou un vote c'est déjà une contrib
        * Faire avec le temps qu'on as, même 3 mois sur 12 de présence c'est déjà de belle contrib

    * README

        * Évolution des readme, ajouter un vrais lien vers la doc
        * Mettre les examples dans le readme si la LIB, quick usage & template & liste of awecodes & liste des projets qui utilisent cette lib pour exemple.
        * mettre un lien vers le contributor guide.
        * mettre un lien vers le waffle
        * mettre un lien vers les snippets

    * Waffle 

        * @grummfy ask to waffle le stats des visites sur le board

    * Snippet

        * lister des snippets à court terme
        * @pierozi ouvrir une issue

    * RulerZ

        * lead par kevin pour bundle SF




