# ORNet Software Protocol Description
ORNet software is a suite of products that can be integrated with Laboratory Information Systems (LIS) to provide advanced functionalities. The software supports a URI protocol launch mechanism to start the ORNet products from within the LIS.

The URI protocol format for launching ORNet products is as follows:
| Product     | Protocol    |
| ----------- | ----------- |
| Surgery      | ornetsurgery:start?{`cmd`}       |
| Pathology   | ornetpathology:start?{`cmd`}        |
| Editor   | orneteditor:start?{`cmd`}        |

The ORNet software supports two commands for launching the products, `lang` and `mode`. The `lang` command allows the user to launch ORNet with a specified language, while the `mode` command forces ORNet to be launched in a supported mode (only for debugging).
## Examples
Here are some examples:

- Launch ORNet Pathology in Finnish language:

```ruby
ornetpathology:start?lang=fi-FI
```
- Launch ORNet Surgery in `auditorium` mode:

```ruby
ornetsurgery:start?mode=auditorium
```
- Launch ORNet Surgery in Finnish language and `normal` mode:

```ruby
ornetsurgery:start?lang=fi-FI&mode=normal
```

It is important to note that the `lang` command does not affect the settings in the database and only changes the language used by ORNet during the session.

## Integrations and cooperation
By following this protocol description, developers of Laboratory Information Systems can integrate their software with the ORNet product family and provide advanced functionalities to their users. We are always open to cooperation and exploring new possibilities to add functionality to the ORNet protocol.
\
\
We understand the importance of collaboration in the software development community, which is why we are excited to work with other companies and developers to enhance the ORNet software suite. We believe that by combining our expertise and resources, we can create innovative solutions that benefit the entire industry.
\
\
If you have any ideas or suggestions for new features or functionalities that could be added to the ORNet protocol, we would love to hear from you. We are always looking for ways to improve our products and services, and we believe that your input can help us achieve this goal.
