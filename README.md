# rakuten
**Devops Challenge**

When you're done, we should be able to type vagrant up and our app will be running and reachable on http port 80 at http://10.10.10.20

**Requirement**:
- The provisioner should clone this github repo into the VM under /webapps/devops
- You should be able to find what system packages are needed by looking through the app
- You should not need to change the app code in any way
- The app should be running as a non-privileged user
- The app should be automatically restarted if crashes or if killed
- The app should maximize all of the available CPUs (have Vagrant virtualize multiple CPUs)
- The related logs should be rotated
- Timezone should be in UTC
