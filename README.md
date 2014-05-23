rancid-linerate
===============

A RANCID module for LineRate load balancer.

#### Installation:
* Add `'linerate' => 'lrancid'` to the vendortable hash in rancid-fe
* Add the `lrancid` file to your rancid bin directory
* Update your `router.db` file, using `linerate` as the device type, like:
        linerate01:linerate:up

#### Other Notes:
Test with RANCID 2.3.8 and LROS 1.6
