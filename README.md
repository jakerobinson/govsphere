# Go API for VMware vSphere (Alpha)

Fully documented and friendly VMWare vSphere API for Go.

### Versions supported
5.5 and previous versions

## Prerequisite
Before attempting to use this API please take some time to familiarize yourself with [VMware VI object model](http://www.doublecloud.org/2010/02/object-model-of-vmware-vsphere-api-a-big-picture-in-2-minutes/)


## CLI installation
`go install`

## API code generation
`$ govsphere generate`

## API definitions generation
The generation process is going to create a file called api.json, relative to the path
from where the command is executed.

`$ govsphere scrape`

Example output:

![](https://i.cloudup.com/sEiUVA9a8L.png)

## Documentation
Start the godoc server and open up your browser: `godoc -http=:6060`

## TODO
1. Generate an Error() function for all vSphere faults to implement golang error interface
2. Implement ManagedObject.currentProperty()
3. Add support for JSON Schema in api.json generation

## License
Copyright 2014 Cloudescape

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
