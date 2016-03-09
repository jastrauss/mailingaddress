# MailingAddress

mailingaddress is simple python library that converts raw address strings into the parts necessary to address mail. The heavy lifting is done by [usaddress], a python library that uses NLP to identify very specific address components. 

[usaddress]: <https://github.com/datamade/usaddress>


## Using mailingaddress

1. Install mailingaddress with [pip]. In a shell,

    [pip]: <http://pip.readthedocs.org/en/latest/quickstart.html>
    ```sh
    $ pip install usaddress
    ```

2. Convert a raw address to a mailing address

    ```sh
        >>> import mailingaddress
        >>> mailingaddress.convert('Jerry Seinfeld, 129 West 81st Street, Apt 5A, New York, New York 12345')
    {
        'name': 'Jerry Seinfeld',
        'address_line_1: '129 West 81st Street',
        'address_line_2: 'Apt 5A',
        'address_line_city: 'New York',
        'address_line_state: 'NY',
        'address_line_zipcode: '12345'
    }
    ```

3. Profit????
