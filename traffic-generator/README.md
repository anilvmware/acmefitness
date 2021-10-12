## Trafiic Generator

### Requirements

1. Needs Python3.6 and above

2. Locust - [Locust](https://docs.locust.io/en/stable/installation.html)

3. ACME Fitness App 

### Steps

1. pip3 install -r requirements.txt

2. locust --host=http://{IP ADDRESS}:{PORT}, where IP_ADDRESS and PORT are the address on which the ACME SHOP App is running. 

3. Navigate to http://localhost:8089

4. Click on 'New Test' and provide the number of users to simulate. 

### Local changes (Oct-'21)

There have been several changes to Locust since the time this document was written. Following are changes/updates to locustfile.py:

 - Deprecation of TaskSequence and replacement with SequentialTaskSet

 - Remove decorator seq_task()

 - Replace class inheritance of TaskSequence with SequentialTaskSet

 - Remove min_wait, max_wait and replace with between()

 - Some of the urls have been updated so that locust cli is:
   /Users/ssharat/Library/Python/3.8/bin/locust "--host=http://127.0.0.1:55767/"

NOTE:
If installing the latest Locust distro. skip Step(1) - versions in requirements.txt are deprecated. 


