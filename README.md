# NAME

Mojolicious::Plugin::Leafletjs - A Mojolicious Plugin

# SYNOPSIS

\# Mojolicious
$self->plugin(
    'Leafletjs' => {
        longitude => '75',
        latitude  => '-0.5'
    }
);

\# Mojolicious::Lite
plugin 'Leafletjs',
  { longitude => '75',
    latitude  => '-0.5'
  };

\# In your template
  <%= leaflet %>
  <%= leaflet\_marker 'marker1', '75.02', '-35.02' %>

# DESCRIPTION

Mojolicious::Plugin::Leafletjs is helpers for integrating simple maps via leafletjs

# HELPERS

## __leaflet__

Accepts the following key/value:

- name => 'map'
- div  => 'map'
- longitude => undef (\*)
- latitude  => undef (\*)
- zoomLevel => 13
- tileLayer => 'map tile png'
- maxZoom => 18
- attribution => 'copyright'

\* Is required

## __leaflet\_marker__

Accepts the following positional arguments:

- marker\_name(\*)
- longitude(\*)
- latitude(\*)
- parent\_map(defaults to 'map')

\* Is required

# TODO

- Add circles
- Add polygons
- Add popups

# CONTRIBUTIONS

Always welcomed! [https://github.com/battlemidget/Mojolicious-Plugin-Leafletjs](https://github.com/battlemidget/Mojolicious-Plugin-Leafletjs)

# AUTHOR

Adam Stokes <adamjs@cpan.org>

# COPYRIGHT

Copyright 2013- Adam Stokes

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
