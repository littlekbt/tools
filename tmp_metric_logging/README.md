# tmp_metric_logging

tmp_metric_logging saves top, vmstat, iostat, mpstat command's output temporary.

## Description
tmp_metric_logging saves temporary output of commands.  
It effective when you want to know the details of server metric.

It supports commands `top -b -n 1`, `vmstat`, `iostat -dmx`, `mpstat -P ALL`.

Once exec commands, writes stdout to /tmp/metric/{command_name}/yyyymmdd_MM.log file.

※ note: /tmp/metric is default. You can change directory by using -f option.

## Require

sysstat, procps package.

## Usage

```
$ sh tmp_metric_logging [-d <duration exec commands>] [-n <num of versions to store>] [-f <path to log dir>] [-t]
```

※ -t: t is dry-run option. if use -t, don't remove old version files.

## Author

[littlekbt](https://github.com/littlekbt)
