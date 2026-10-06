# Boat Chart

A phone chart page for boat jobs: satellite, the official AHO chart and OpenSeaMap beacons, live GPS
with speed in knots, 6 knot zone warnings, the planned route and an ETA to the next stop, and
time stamps with a GPX track to prove job times.

Not for navigation. The boat's own chart plotter stays the primary.

The page holds no job details. A job is opened from a link made by the quoter (`chart.py link`),
which carries the route in the part of the address after `#`, and browsers never send that part to
the server. Track and stamps stay on the phone.

`index.html` is built by `chart.py page` from the quoter's template and zone data; edit those, not
this file.
