# groovy-cli-gradle-sybase-index

## Description
Creates a small database table
called `dog`. This table, `dog`, has 2 non-clustered
index and has been normalized to 3NF.
All output normally
seen in a terminal will be in `groovy-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- docker-wait
- groovy
- gradle
  - log4j
  - sybase driver

## Docker stack
- gradle:jdk11
- datagrip/sybase

## To run
`sudo ./install.sh -u`
Creates groovy-srv/log

## To stop
`sudo ./install.sh -d`
Removes groovy-srv/log

## For help
`sudo ./install.sh -h`

## Credit
- [Sybase driver and connection example](https://razorsql.com/docs/help_sybase.html)
