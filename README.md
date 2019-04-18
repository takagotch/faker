### faker
---
.rb
https://github.com/stympy/faker

.py
https://github.com/joke2k/faker

```sh
gem install faker
gem 'facker', :git => 'https://github.com/stympy/faker.git', :branch => 'master'
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

```
