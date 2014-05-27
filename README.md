rancid-linerate
===============

A [RANCID](http://www.shrubbery.net/rancid/) module for [LineRate](https://linerate.f5.com/) load balancer.

#### Installation:
* Add `'linerate' => 'lrancid'` to the vendortable hash in rancid-fe
* Add the `lrancid` file to your rancid bin directory and make sure the rancid user has execute permissions
* Update your `router.db` file, using `linerate` as the device type, like:

        linerate01:linerate:up
* Update your `.cloginrc` with something like:

        add method linerate01 {ssh}
        add user linerate01 {admin}
        add password linerate01 {changeme}
        add autoenable linerate01 {1}

#### Other Notes:
Currently, there is a limitation where the hostname of the LROS proxy has to be the same as the hostname defined router.db and .cloginrc.

Tested with RANCID 2.3.8 and LROS 1.6
