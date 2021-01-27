NLog.Targets.Fluentd
====================

NLog.Targets.Fluents is a custom target of [NLog](https://github.com/nlog/NLog) that emits the log entries to a [fluentd](http://www.fluentd.org/) node.

Settings
--------

Setting                     | Description                                                                                                   | Example            
--------------------------- | ------------------------------------------------------------------------------------------------------------  | -------------------
host                        | Host name of the fluentd node                                                                                 | example.local
port                        | Port number of the fluentd node                                                                               | 24224
tag                         | Fluentd tag name                                                                                              | windowshost
noDelay                     | Enable Nagle's algorithm                                                                                      | true
sendBufferSize              | Send buffer size                                                                                              | 8192
sendTimeout                 | Send timeout                                                                                                  | 2
lingerEnabled               | Wait for all the data to be sent when closing the connection                                                  | false
lingerTime                  | Linger timeout                                                                                                | 2
emitStackTraceWhenAvailable | Emit a stacktrace for every log entry when available                                                          | false
includeEventProperties      | Include structured logging parameters from LogEvent properties.                                               | false
includeMdlc                 | Include structured logging parameters from `MappedDiagnosticsLogicalContext`.                                 | false
excludeProperties           | Comma separated string with names which properties to exclude. Only used when IncludeAllProperties is *true*. | property1,property2

Read more about [Contexts in NLog](https://github.com/NLog/NLog/wiki/Context).

License
-------

NLog.Targets.Fluentd

Copyright (c) 2014 Moriyoshi Koizumi and contributors.

This software is licensed under the Apache License, Version 2.0 (the "License");
you may not use this software except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
