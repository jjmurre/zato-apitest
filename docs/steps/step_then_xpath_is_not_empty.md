
Then XPath "{xpath}" isn't empty
=============================================================================================================

Usage example
-------------

```
Feature: zato-apitest docs

Scenario: Then XPath "{xpath}" isn't empty

    Given address "http://apitest-demo.zato.io"
    Given URL path "/demo/xml2"
    Given format "XML"
    Given request is "<req><howdy>foo</howdy></req>"

    When the URL is invoked

    Then XPath "//not-empty" isn't empty
```

Discussion
----------

(None)