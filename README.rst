===========================
 sphinxcontrib-peopledomain
===========================

Sphinx domain for describing people.

If you use sphinx as blog, you can use this domain to manange your friends link.

Installation
============

::

    pip install sphinxcontrib-peopledomain


Configuration
=============

Add ``'sphinxcontrib.peopledomain'`` to the ``extensions`` list in ``conf.py``::

    extensions = [ 'sphinxcontrib.peopledomain' ]


Usage
=====

For now, this package provides a domain named ``ppl``.

To create a description of your friend, use ``friend`` directive::

    .. ppl:friend:: SilverRainZ
       :homepage: https://silverrainz.me

       Human.

Then you can use role ``:ppl:friend:`SilverRainZ``` to refer him.
It will be rendered as "@SilverRainZ" with the appropriate link.

Changelog
=========

0.1
  Provide the "ppl" domain, "friend" directive and "friend" role.
