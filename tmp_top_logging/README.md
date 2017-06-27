# tmp_top_logging

tmp_top_logging saves temporary output of top command.

# Description
tmp_top_logging saves temporary output of top command.  
It effective when you want to know the details of server metric.

# Require
On centos: tmpwatch  
On ubuntu: tmpreaper 

# Usage

```
$ sh tmp_top_logging [-d <duration exec top command>] [-s <store num of versions>] [-f <path to log dir>]
```

use as backgroud job.
```
$ nohup sh tmp_top_logging &
```

# Author

[littlekbt](https://github.com/littlekbt)
