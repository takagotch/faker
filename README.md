### faker
---
https://github.com/stympy/faker

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

```




