# NAME

Mojolicious::Plugin::Leafletjs - A Mojolicious Plugin

# SYNOPSIS

    # Mojolicious
    $self->plugin(
      'Leafletjs' => {
          longitude => '75',
          latitude  => '-0.5'
      }
    );

    # Mojolicious::Lite
    plugin 'Leafletjs',
    { longitude => '75',
      latitude  => '-0.5'
    };
    # In your template
    <%= leaflet %>
    <%= leaflet_marker 'marker1', '75.02', '-35.02' %>

# DESCRIPTION

Mojolicious::Plugin::Leafletjs is helpers for integrating simple maps via leafletjs

# HELPERS

## __leaflet__

Accepts the following options:

- name

    Name of map variable

- longitude

    Longitude

- latitude

    Latidude

- cssid

    CSS id of map

- zoomLevel

    Map zoomlevel

- tileLayer

    URL of map tile layer, defaults to a cloudmade.com tile

- maxZoom

    Max zoom into the map

- attribution

    Show some love for the leaflet team, openmap, and cloudmade map tiles

## __leaflet\_marker__

Accepts the following positional arguments:

- marker\_name

    Name of Map variable

- longitude

    Longitude

- latitude

    Latitude

- parent\_map

    Map variable

## __leaflet\_popup__

Accepts the following positional arguments:

- marker\_name

    Variable name of marker

- message

    Message to display in popup

# TODO

- Add circles
- Add polygons

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
