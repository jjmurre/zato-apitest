
Given XPath "{xpath}" in request is a random date after "{date_start}" "{format}"
=============================================================================================================

Usage example
-------------

```
Feature: zatoapi-test docs

Scenario: Given XPath "{xpath}" in request is a random date after "{date_start}" "{format}"

    Given address "http://apitest-demo.zato.io"
    Given URL path "/demo/XML"
    Given HTTP method "POST"
    Given format "XML"
    Given request "demo.xml"
    Given XPath "//howdy" in request is a random date after "2019-07-25" "default"

    When the URL is invoked

    Then status is "200"
```

Discussion
----------

* The format "default" is always available. Its value is "YYYY-MM-DDTHH:mm:ss".
* Use format "YYYY-MM-DD" to specify "{date_start}".