# mstats
a simple script to collect OS level performance metrics for Linux
metrics include:
- CPU
- filesystem
- diskstats (io metrics)
- network protocol (tcp, udp, ip)
- network interface stats
- load average
- per-process stats like user/sys CPU, I/O requests, page fault etc.

## requirements
 Python 2.6+ (not sure if 3.0 works, I haven't test it), which should be included in most Linux distro by default
## usage
    python mstats -h
    Usage: mstats [options]

    Options:
      -h, --help            show this help message and exit
      -c FILE, --config=FILE
                            configuration file (no default value)
      -l LOGLEVEL, --loglevel=LOGLEVEL
                            set log level, can be debug, info, warn, error or
                            critical (default warn)

## configuration
 see mstats.json.example, remember to remove comments
## installation
 copy/download the mstats file to somewhere on your target machine, modify the mstats.json file and run the script:

    python mstats -c mstats.json >> mstats.log

## screen shot
[[screenshot.png]]
