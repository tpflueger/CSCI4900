# CSCI4900 [![Build Status](https://travis-ci.org/tpflueger/CSCI4900.svg?branch=master)](https://travis-ci.org/tpflueger/CSCI4900)

## To install
`pip install .` within top-level of project

Note - Current setup doesn't install [DoSOCSv2](https://github.com/DoSOCSv2/DoSOCSv2) completely. You will need to follow their instructions first before trying to install current project for it to work.

## Usage
Pass pom.xml to be parsed, domaven will then pass all the parsed dependencies to DoSOCSv2 with relationship info:

    $ domaven ./path/to/pom.xml

## System Description
Python script that connects Maven to DoSOCS. Uses Maven to find out project-level dependencies based on passed pom.xml. A tree is constructed of the hierarchy from parent package downward. All the packages are then given to DoSOCSv2 to be stored into the the database along with the relationship info information which pertains to the SPDX schema.

## Development Environment
- UBUNTU 14.04
- Python 2.7
- DoSOCSv2

## Communication Management Plan
- Email
- Github
- 2 meetings a week (Tuesdays/Thursdays)

## Dataflow diagram of the system
![dataflow-diagram](https://cloud.githubusercontent.com/assets/8797790/13299389/94a17488-db00-11e5-93ad-13b4e96eb395.png)

## SPDX diagram of database
![SPDX-diagram](https://cloud.githubusercontent.com/assets/2850506/13796701/2f0e8508-ead6-11e5-86c9-62c93beed600.png)

## License

MIT © Aarjav Chauhan, Tyler Pflueger

CC-BY-SA-4.0 © Aarjav Chauhan, Tyler Pflueger
