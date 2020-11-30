# Copyright
Copyright (C) 2020, TietoEVRY

# License
This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed with this file, You can obtain one at http://mozilla.org/MPL/2.0/.

# Overview
## Build instructions
The intention is to maintain two build systems with a preference to support Android.bp.
Each module has its own Android.bp and gradle file.

### Gradle
From the directory of the desired module (_vssservice_ for the service, _vssservice-client_ for the client):
```
./gradlew assembleDebug
```

### Android build system

Deploy the repository inside AOSP tree i.e. `/vendor/genivi/packages/vehicleplugin-vss-graphql` and call make from the top of the repo:
```
make com.tieto.vehicleplugin.graphql
```
