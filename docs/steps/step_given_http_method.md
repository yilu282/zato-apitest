
Given HTTP method "{method}"
=============================================================================================================

Usage example
-------------

```
Feature: zato-apitest docs

Scenario: Given HTTP method "{method}"

    Given address "http://apitest-demo.zato.io"
    Given URL path "/demo/json"
    Given HTTP method "PATCH"

    When the URL is invoked

    Then status is "405"
```

Discussion
----------

GET is used if not method is specified