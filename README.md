# GTFS Diff : specification to list differences between GTFS files

## Goal
GTFS Diff aims at providing a universal and unified way to list differences between two GTFS files. It is designed to be easily understandable by humans, but also easily produced and processed by computers.

## Context
[transport.data.gouv.fr](transport.data.gouv.fr) is the French National Access Point for mobility data. It is operated by the French Ministry of Transportation. The platform gives access to a variety of mobility data, including a number of GTFS files.

It happens frequently that companies or individuals using this data modify it. For example to correct spelling mistakes in a stop name, add color to routes or wheelchair information.

Every time a GTFS file is updated by the producer with a recent schedule, those corrections need to be applied again. We lack a universal way to list a series of modifications with the corresponding explanations about the change.

It also happens that data users share their enhanced GTFS file on our platform. We then lack a way to easily understand the changes they made. If two users share their own modified version of a GTFS, we lack a way to merge their respective changes into a single file.

It is also hard for reusers to review the changes made to a given GTFS file by its official producer, making it harder to understand the impact of the changes on their systems.

## Resources
- the GTFS Diff specification
- Online tool to generate a GTFS Diff on transport.data.gouv.fr/tools/
- Source code of the implementation (in Elixir)