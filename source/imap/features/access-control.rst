..  Note to documentation authors, this document is also included in the
    administrator guide's access control section.

==============
Access Control
==============

.. NOTE::

    Cyrus IMAP documentation is a work in progress. The completion of
    this particular part of the documentation is pending the resolution
    of :task:`51`.

Cyrus IMAP features powerful access control compliant with :rfc:`2086`,
:rfc:`4314`, :rfc:`5257` and :rfc:`5464`.

.. _imap-features-access-control-lists-discretionary:

Discretionary Access Control
============================

Cyrus IMAP employs discretionary access control, meaning that users
themselves are in charge of what folders are shared, and with whom.

Two means exist to suppress sharing folders between users:

#.  Revoke the :ref:`imap-admin-access-control-right-a` (administration)
    right on all mailboxes in the personal namespace for each user.

#.  Suppress the listing of the
    :ref:`imap-features-namespaces-other-users` by enabling
    ``disable_user_namespace`` in :manpage:`imapd.conf(5)`.

.. seealso::

    *   :ref:`imap-admin-access-control-lists-rights-reference`
    *   :ref:`imap-admin-access-control-combining-rights`

.. toctree::
    :hidden:
    :glob:

    access-control/*