
Given namespace prefix "{prefix}" of "{namespace}"
=============================================================================================================

Usage example
-------------

```
Feature: zatoapi-test docs

Scenario: Given namespace prefix "{prefix}" of "{namespace}"

    Given address "http://apitest-demo.zato.io"
    Given URL path "/demo/XML"
    Given format "XML"
    Given namespace prefix "cust" of "http://example.com/crm"

    When the URL is invoked

    Then status is "200"
```

Discussion
----------

Sets a namespace prefix that can be used in subsequent XPath expressions.