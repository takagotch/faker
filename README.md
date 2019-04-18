### faker
---
.rb
https://github.com/stympy/faker

.py
https://github.com/joke2k/faker

```sh
gem install faker
gem 'facker', :git => 'https://github.com/stympy/faker.git', :branch => 'master'

tox
python -m faker > docs.txt
faker address
faker -l de_DE address
faker profile ssn,birthdate
faker -r=3 -s=";" name
pip install Faker
```

```ruby
require 'facker'
Faker::Name.name
Faker::Internet.email

Faker::Name.unique.name

Faker::Name.unique.clear
Faker::UniqueGenerator.clear

Faker::Lorem.unique.exclude :string, [6], %w[azerty wxcvbn]

Faker::Config.random = Random.new(42)
Faker::Company.bs
Faker::Company.bs
Faker::Config.random = Random.new(42)
Faker::Company.bs
Faker::Company.bs

Faker::Config.random = nil
Faker::Config.random.seed
Faker::Company.bs
```

```yml
en-qu-ocker:
  faker:
    name:
      first_name: [Charlotte, Ava, Chloe, Emily]
      ocker_first_name: [Bazza, Bluey, Davo, Johno, Shano, Shazza]
      region: [South East Queensland, Wide Bay Burnett, Margaret River, Port Pirie, Gippslnad, Elizabeth, Barossa]

```


```ruby
irb
require 'rubygems'
require 'faker'

Faker::Address.city
Faker::Address.street_name
Faker::Address.street_address
Faker::Address.secondary_address
Faker::Address.zip_code
Faker::Address.zip
Faker::Address.postcode
Faker::Address.street_suffix
Faker::Address.city_suffix
Faker::Address.city_prefix
Faker::Address.state_abbr
Faker::Address.state
Faker::Address.state
Faker::Address.country
Faker::Address.country_code

```


```py
from faker import Faker
fake = Faker()
fake.seed(4321)

print(fake.name())

from faker import Faker
fake = Faker()
fake.seed_instance(4321)

print(fake.name())


import factory
from myapp.models import Book

class BookFactory(factory.Factory):
  class Meta;
    model = Book
    
   title = facotry.Faker('sentence', nb_words=4)
   author_name = factory.Faker('name')

from faker import Faker
fake = Faker()
fake.random
fake.randomgetstate()


form faker.providers import BaseProvider

class Provider(BaseProvider):
  def foo(self):
    return 'bar'
    
fake.add_provider(Provider)

fake.foo()


from faker import Faker
fake = Faker()

my_word_list = [
'danish','cheesecake','sugar',
'Lollipop','wafer','Gummies',
'sesame','Jelly','beans',
'pie','bar','Ice','oat',]

faker.sentence()

fake.sentence(ext_word_list=my_word_list)


from faker import Faker
fake = Faker()

from faker.providers import BaseProvider

class Provider(BaseProvider):
  def foo(self):
    return 'bar'
    
fake.add_provider(Provider)

fake.foo()

from faker import Faker
from faker.providers import internet

fake = Faker()
fake.add_provider(internet)

print(fake.ipv4_private())

from faker import Faker
fake = Faker('it_IT')
for _ in range(10):
  print(fake.name())

for _ in range(10):
  print(fake.name())
  
  
from faker import Faker
fake = Faker()

fake.name()
fake.address()
fake.text()
```
