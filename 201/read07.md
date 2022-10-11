# Object-Oriented Programming, HTML Tables

## Domain Modeling

1. A **domain model** that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## HTML Table Basics

1. **Tables** should not be used for page layouts for the following reasons:

    - Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.
    - Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
    - Tables are not automatically responsive: When you use proper layout containers (such as <header>, <section>, <article>, or <div>), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.
2. 3 different semantic elements in a table are:

    - **tr** stops a row from growing and starts placing subsequent cells on a second row, the **<tr>** element 'tr' stands for 'table row'.
    - A **<td>** element ('td' stands for 'table data') is the smallest container inside a table and is a table cell.
    - To recognize the table headers as headers, both visually and semantically, you can use the **<th>** element ('th' stands for 'table header').
3. The term this differs when used in an object literal versus when used in a constructor because Objects created using object literals are singletons.

### Sources

- <https://github.com/codefellows/domain_modeling#domain-modeling>
- <https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics>
- <https://ui.dev/beginners-guide-to-javascript-prototype>

[Back To Home](../README.md)
