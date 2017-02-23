This simple module exposes SimpleTest test cases to be executed on a site
to help identify potential issues.

A custom test case type (AuditTestCase) has been created extending the default
DrupalWebTestCase to avoid the creation of a dedicated environment. That means
all the tests are performed directly on the environment the module is enabled
on. The test cases should not write or edit anything in the database unless the
reporting messages in the Simpletest table.