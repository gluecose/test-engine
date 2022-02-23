# test-engine
Test Engine is the logic that drives the interoperability testing.

# Contents
Test Engine repository of Gluecose system comprises:

1. Database schema, where each DB row will have information about specific COSE implemenation, feature supported, level of support etc.

2. A set of queries that can be executed by users, to fetch specific information about a COSE library from the database.

3. A SQLite DB hosting the actual data.

4. Logic that executes an Automated Compliance Runner(ACR), takes the output of the run and re-shapes the output data in a format understood by the DB Schema and pushes the data into the DB.

5. Collects Logs of execution and saves it in a pre-defined location. Possesses a feature to send an automated email to the library provider, in case there is a failure during test execution.


