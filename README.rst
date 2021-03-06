ForgeryPy
=========

ForgeryPy is an easy to use forged data generator. It's a (somewhat incomplete)
port of ``forgery`` Ruby gem.

This is a fork of Tomek Wójcik's `original ForgeryPy port
<https://github.com/tomekwojcik/ForgeryPy>`_, fixed to work under
``Python 3`` and extended with the new dictionaries from the original
Ruby gem ``forgery``.


Example usage
-------------

>>> import forgery_py
>>> forgery_py.address.street_address()
'4358 Shopko Junction'
>>> forgery_py.basic.hex_color()
'3F0A59'
>>> forgery_py.currency.description()
'Slovenia Tolars'
>>> forgery_py.date.date()
datetime.date(2012, 7, 27)
>>> forgery_py.internet.email_address()
'brian@zazio.mil'
>>> forgery_py.lorem_ipsum.title()
'Pretium nam rhoncus ultrices!'
>>> forgery_py.name.full_name()
'Mary Peters'
>>> forgery_py.personal.language()
'Hungarian'


Full List of methods
--------------------

+------------------------------------------------------+-------------------------------------------+
|Method                                                | Example Output                            |
+======================================================+===========================================+
| forgery_py.address.city()                            | 'Larkspur'                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.continent()                       | 'North America'                           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.country()                         | 'Belgium'                                 |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.phone()                           | '5-(721)114-0241'                         |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.state()                           | 'Kansas'                                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.state_abbrev()                    | 'LA'                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.street_address()                  | '4 Eastlawn Junction                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.street_name()                     | 'Dexter'                                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.street_number()                   | '1'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.street_suffix()                   | 'Park'                                    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.address.zip_code()                        | '65843-3832'                              |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.hex_color()                         | '6D1F5B'                                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.hex_color_short()                   | '05C'                                     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.text()                              | 'ncvgIY0pGKGHv'                           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.boolean()                           | True                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.color()                             | 'Red'                                     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.encrypt()                           | 'fc0d835dd4e4df144a33a6a346298b0f23dcd14a'|
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.frequency()                         | 'Never'                                   |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.number()                            | 5                                         |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.basic.password()                          | 'KcLBHCv6'                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.credit_card.check_digit(num)              | 5                                         |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.credit_card.number()                      | 343682330855371                           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.credit_card.type()                        | 'American Express'                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.currency.code()                           | 'CHF'                                     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.currency.description()                    | 'Canada Dollars'                          |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.date.date()                               | datetime.date(2016, 11, 8)                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.date.day()                                | 4                                         |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.date.day_of_week()                        | 'Thursday'                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.date.month()                              | 'September'                               |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.date.year()                               | 2021                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.email.address()                           | 'gsmith@kamba.org'                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.email.body()                              | 'Lorem ipsum dolor sit amet, ...'         |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.email.subject()                           | 'Lorem Ipsum Dolor Sit Amet...'           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.latitude()                            | -8.095096815540515                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.latitude_degrees()                    | -49                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.latitude_direction()                  | 'N'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.latitude_minutes()                    | 14                                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.latitude_seconds()                    | 45                                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.longitude()                           | -22.56746406884514                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.longitude_degrees()                   | 100                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.longitude_direction()                 | 'W'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.longitude_minutes()                   | 47                                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.geo.longitude_seconds()                   | 41                                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.cctld()                          | 'om'                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.domain_name()                    | 'edgepulse.name'                          |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.email_address()                  | 'lillian@flashpoint.biz'                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.email_subject()                  | 'Lorem Ipsum Dolor Sit Amet...'           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.ip_v4()                          | '96.36.71.94'                             |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.top_level_domain()               | 'gov'                                     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.internet.user_name()                      | 'earl'                                    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.paragraph()                   | 'In hac habitasse platea dictumst...'     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.paragraphs()                  | 'Nam nulla. Phasellus sit amet erat.'     |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.sentence()                    | 'Quisque porta volutpat erat.'            |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.sentences()                   | 'Duis consequat... Integer non velit...'  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.title()                       | 'Vestibulum proin tristique lobortis!'    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.word()                        | 'maecenas'                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.words()                       | 'platea cubilia pede et ultrices congue'  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.character()                   | 'l'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.characters()                  | 'lorem ipsu'                              |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.lorem_ipsum_characters()      | 'lorem ipsum dolor sit amet...'           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.lorem_ipsum_words()           | ["lorem", "ipsum", "dolor", ...]          |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.lorem_ipsum.text()                        | 'Lorem ipsum dolor sit amet...'           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.monetary.formatted_money()                | '$5.49'                                   |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.monetary.money()                          | '9.20'                                    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.company_name()                       | 'Dabtype'                                 |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.female_first_name()                  | 'Katherine'                               |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.first_name()                         | 'Jose'                                    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.full_name()                          | 'James Williamson'                        |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.industry()                           | 'Machine Tools & Accessories'             |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.job_title()                          | 'Operator'                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.job_title_suffix()                   | 'I'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.last_name()                          | 'Henry'                                   |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.location()                           | 'Kwik-E-Mart'                             |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.male_first_name()                    | 'Cheryl'                                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.suffix()                             | 'IV'                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.name.title()                              | 'Ms'                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.personal.abbreviated_gender()             | 'F'                                       |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.personal.gender()                         | 'Male'                                    |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.personal.language()                       | 'Tsonga'                                  |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.personal.race()                           | 'Sri Lankan'                              |
+------------------------------------------------------+-------------------------------------------+ 
| forgery_py.personal.shirt_size()                     | 'XS'                                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.time.zone()                               | 'Amsterdam'                               |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.account_number()              | 56335652786612121479                      |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.bik()                         | 046533860                                 |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.inn()                         | 7366543467                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.legal_inn()                   | 7822838630                                |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.legal_ogrn()                  | 3483465598635                             |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.ogrn()                        | 666325227817763                           |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.person_inn()                  | 451559765443                              |
+------------------------------------------------------+-------------------------------------------+
| forgery_py.russian_tax.person_ogrn()                 | 195478617554621                           |
+------------------------------------------------------+-------------------------------------------+

TODO
----

+------------------------------------------------------+-------------------------------------------+
| Method Missed                                        | Example Output                            |
+======================================================+===========================================+
| ...                                                  | ...                                       |
+------------------------------------------------------+-------------------------------------------+


Credits
-------

The project uses dictionary files from `forgery Ruby gem <https://github.com/sevenwire/forgery>`_.


License
-------

MIT-style, see LICENSE
