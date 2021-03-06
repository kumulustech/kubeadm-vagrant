# A Vagrantfile to deploy a multi-node Kubernetes with kubeadm via bash

Vagrantfile supports only ubuntu and virtualbox at the moment
it's based on the Vagrantfile from the kubernetes git repository.

You can adjust the number of client nodes by changing the NUM_NODES
environment variable.

To launch the environment, just do:

  `vagrant up`

Once the system has launched, you should be able to verify
the kubernetes environment by logging into the master node with:

  `vagrant ssh master`
  
 Then:
  
  `kubectl get nodes`

Examples for the KUB-100 class are in the example_files directory

======
 Copyright 2017, 2018 Kumulus Technologies
 Copyright 2017, 2018 Robert Starmer

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
