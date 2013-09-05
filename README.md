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

# AUTHOR

Adam Stokes <adamjs@cpan.org>

# COPYRIGHT

Copyright 2013- Adam Stokes

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
