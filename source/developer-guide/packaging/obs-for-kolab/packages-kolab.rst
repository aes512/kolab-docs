==============
Kolab Packages
==============

chwala
======

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development chwala -F -` << EOF
    <package name="chwala">
        <title>chwala</title>
        <description>
            Kolab Groupware Integrated File Storage Interfaces
        </description>
        <url>http://chwala.org</url>
    </package>
    EOF

.. include:: packages/chwala.txt

cyrus-imapd
===========

While the Kolab Groupware community is not strictly upstream for the Cyrus IMAP
package, Kolab Systems staff actively participates in upstream development.

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development cyrus-imapd -F -` << EOF
    <package name="cyrus-imapd">
        <title>cyrus-imapd</title>
        <description>Cyrus IMAP server</description>
        <url>http://www.cyrusimap.org</url>
    </package>
    EOF

.. rubric:: See Also

*   :ref:`packages-dependencies-jansson` (Build dependency as of
    **cyrus-imapd-2.5+**)

.. include:: packages/cyrus-imapd.txt

iRony
=====

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development iRony -F -` << EOF
    <package name="iRony">
        <title>iRony</title>
        <description>
            DAV Access Provider for Kolab Groupware
        </description>
        <url>http://kolab.org/about/iRony</url>
    </package>
    EOF

.. include:: packages/iRony.txt

kolab
=====

The **kolab** package is a meta-package for mainstream distributions
such as Debian, Enterprise Linux, Fedora, openSUSE and Ubuntu.

It is used to enable a system administrator to quickly install a
complete, default Kolab Groupware stack.

For non-mainstream distributions, such as Univention Corporate Server,
the **kolab** package, and/or any of its sub-packages, includes the
routines needed to integrate in to the standing solution(s) for
system management.

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab -F -` << EOF
    <package name="kolab">
        <title>kolab</title>
        <description></description>
        <url>http://kolab.org/about/kolab</url>
    </package>
    EOF

.. include:: packages/kolab.txt

kolab-freebusy
==============

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab-freebusy -F -` << EOF
    <package name="kolab-freebusy">
        <title>kolab-freebusy</title>
        <description></description>
        <url>http://kolab.org/about/kolab-freebusy</url>
    </package>
    EOF

.. include:: packages/kolab-freebusy.txt

kolab-selinux
===============

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab-selinux -F -` << EOF
    <package name="kolab-selinux">
        <title>kolab-selinux</title>
        <description></description>
        <url>http://kolab.org/about/kolab-selinux</url>
        <build>
            <disable/>
        </build>
    </package>
    EOF

.. include:: packages/kolab-selinux.txt

kolab-syncroton
===============

ActiveSync server-side implementation, based on the Syncroton libraries.

**kolab-syncroton** ships vendorized copies of the following:

*   :file:`lib/ext/Roundcube/`

    Originating as :file:`/usr/share/roundcubemail/program/lib/Roundcube/`,
    :file:`lib/ext/Roundcube/` should be made a symbolic link to the
    original path. Therefore, installing **kolab-syncroton** must also
    install **roundcubemail**.

*   :file:`lib/plugins/kolab_auth/`

    The Roundcube plugin for Kolab Authentication originates at
    :file:`/usr/share/roundcubemail/plugins/kolab_auth/`, from the
    **roundcubemail-plugins-kolab** package. :file:`lib/plugins/kolab_auth/`
    itself should not be made a symbolic link, however. Instead, its
    contents should be. This would include :file:`kolab_auth.php`,
    :file:`config.inc.php`, and other files and directories.

*   :file:`lib/plugins/kolab_folders/`

*   :file:`lib/plugins/libkolab/`

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab-syncroton -F -` << EOF
    <package name="kolab-syncroton">
        <title>kolab-syncroton</title>
        <description></description>
        <url>http://kolab.org/about/kolab-syncroton</url>
    </package>
    EOF

.. include:: packages/kolab-syncroton.txt

kolab-utils
===========

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab-utils -F -` << EOF
    <package name="kolab-utils">
        <title>kolab-utils</title>
        <description></description>
        <url>http://kolab.org/about/kolab-utils</url>
    </package>
    EOF

.. include:: packages/kolab-utils.txt

kolab-webadmin
==============

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development kolab-webadmin -F -` << EOF
    <package name="kolab-webadmin">
        <title>kolab-webadmin</title>
        <description></description>
        <url>http://kolab.org/about/kolab-webadmin</url>
    </package>
    EOF

.. include:: packages/kolab-webadmin.txt

libcalendaring
==============

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development libcalendaring -F -` << EOF
    <package name="libcalendaring">
        <title>libcalendaring</title>
        <description>
            Frankenstein module to avoid dependencies on most of KDE
        </description>
        <url>http://kolab.org/about/libcalendaring</url>
    </package>
    EOF

.. include:: packages/libcalendaring.txt

libkolab
========

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development libkolab -F -` << EOF
    <package name="libkolab">
        <title>libkolab</title>
        <description></description>
        <url>http://kolab.org/about/libkolab</url>
    </package>
    EOF

.. include:: packages/libkolab.txt

libkolabxml
===========

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development libkolabxml -F -` << EOF
    <package name="libkolabxml">
        <title>libkolabxml</title>
        <description></description>

        <url>http://kolab.org/about/libkolabxml</url>
    </package>
    EOF

.. include:: packages/libkolabxml.txt

pykolab
=======

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development pykolab -F -` << EOF
    <package name="pykolab">
        <title>pykolab</title>
        <description></description>
        <url>http://kolab.org/about/pykolab</url>
    </package>
    EOF

.. include:: packages/pykolab.txt

roundcubemail
=============

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development roundcubemail -F -` << EOF
    <package name="roundcubemail">
        <title>roundcubemail</title>
        <description></description>
        <url>http://kolab.org/about/roundcubemail</url>
    </package>
    EOF

.. include:: packages/roundcubemail.txt

roundcubemail-plugins-kolab
===========================

.. parsed-literal::

    # :command:`osc meta pkg Kolab:Development roundcubemail-plugins-kolab -F -` << EOF
    <package name="roundcubemail-plugins-kolab">
        <title>roundcubemail-plugins-kolab</title>
        <description></description>
        <url>http://kolab.org/about/roundcubemail-plugins-kolab</url>
    </package>
    EOF

.. include:: packages/roundcubemail-plugins-kolab.txt
