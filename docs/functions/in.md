---
layout: with-sidebar
sidebar: documentation
title: in(...)

type: function
datatypes:
- text 
- number
- double
- money
- floating_timestamp
versions:
- 2.1
description: Matches values in a given set of options
parent_paths: 
- /docs/functions/
parents: 
- SoQL Function Listing 
---

{% include function_header.html %}

The `in(...)` function is used within the `$where` parameter to match against a set of possible values. For example, to match on the `THEFT`, `ROBBERY`, and `INTIMIDATION` values in the [Chicago Crimes](http://data.cityofchicago.org/d/6zsd-86xi):

{% include tryit.html domain='data.cityofchicago.org' path='/resource/6zsd-86xi.json' args="$where=primary_type in('THEFT', 'ROBBERY', 'INTIMIDATION')" %}
