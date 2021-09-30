# ProtonVPN-Server-Checker

## Description

This little script asks the ProtonVPN-API for current information (i.e. the server load) about their servers and tells you, which one is the fastest to connect to.

## Usage

```bash
vpn-server [options]
```

### Options

```bash
        -t <type>        select prefered type of server
                      - free
                      - standard (this is the default value)
                      - secure
                      - tor

    following still in progress, has no effect
    -------------------------------------------------------------------------------
        -c <country-code>    select prefered country (2-digit country-code)

        -n <amount>        get this amount of fastest servers as a result

        -s <server>        check only the given server
    -------------------------------------------------------------------------------
```

## Things, I still have to do

- include a check, whether a chosen country even is available on ProtonVPN

- filter servers related to chosen country

- list amount of servers as result

- fully implement the quality check for a specific server (to know, if it still is good enough)

## Things, I want to add in the future

- check for fastest country

## Dependencies

- curl

- jq

- awk

- ripgrep (maybe I will simplify this to grep in a future version)
