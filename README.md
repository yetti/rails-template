# rails template

This is a template for a Rails 7 application.

## Pre-requisites

* Podman or Docker
* `dip` gem

## Setup

1. Clone the repository from source control.
2. Make sure to have Podman/Docker running.
3. Open a terminal and navigate to the project directory.
4. Execute `dip provision` in the terminal.

## Running the app

1. `bin/dev`

## Tests and CI

1. `bin/ci` contains all the tests and checks for the app
2. `tmp/test.log` will use the production logging format *not* the development one.

## Production

* All runtime configuration should be supplied in the UNIX environment
* Rails logging uses `lograge`. `bin/setup help` can tell you how to see this locally.
