# casymir-toolkit README

## require 'casy'
https://support.casymir.ch/wiki/doku.php?id=support:casymir_intern:tooldoc:lua:luacasy

## require 'setup'
https://support.casymir.ch/wiki/doku.php?id=support:casymir_intern:tooldoc:lua:setup
```lua
setup_conf = {
    Description='Local Directory Watcher Setup',

    { Key='DW_ACTIVE', 
        Description='Ueberwachung aktiv (J/N)', 
        Default='J', Values={'^J$','^N$'}, Upper=true },

    { Key='DW_VERBOSE', 
        Description='Loglevel (0-9)', Default='1', Values={'^[0-9]$'} },

    { Key='ADMIN_MAIL', 
        Description='Mailadresse für Probleme', Default='kommerz' },

    { Key='WORK_DIR', 
        Description='Arbeits-Verzeichnis für FTP Downloads', Default='/tmp' },

    { Key = 'WATCH_SLEEP_LOOP', 
        Description='Sleep-Dauer zwischen zwei vollen Durchgängen (sec)', 
        Default=5, Values={'^[0-9]+$'} },

    { SubKey = 'LOCAL1', Description = 'Job 1', Active = 'Yes',
        { Key='ADMIN_MAIL', Description='Mailadresse für Probleme', Default='kommerz' },
    },
    { SubKey = 'LOCAL2', Description = 'Job 2', Active = 'Yes',
        { Key='ADMIN_MAIL', Description='Mailadresse für Probleme', Default='kommerz' },
    },
}
```

## require 'getopt'
https://support.casymir.ch/wiki/doku.php?id=support:casymir_intern:tooldoc:lua:getopt

## https://www.opag.ch/files/gtkdoc/opg_sys/modules/
- `sys.opg_mt_*` ausgelassen