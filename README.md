Random Famous Phrase gem
===========================
How to create a gem ?
__________________________
create a gem with gemname_username like random_famous_phrase_astux7
```
% tree
.
├── random_famous_phrase.gemspec
└── lib
    └── random_famous_phrase.rb
```

+ cat lib/random_famous_phrase.rb
```
class RandomFamousPhrase
  def self.show
    'It should work - By Asta'
  end
end
```
+ cat random_famous_phrase.gemspec
```
Gem::Specification.new do |s|
  s.name        = 'random_famous_phrase'
  s.version     = '0.0.0'
  s.date        = '2014-04-13'
  s.summary     = 'Gives Random famous phrase, image'
  s.description = 'Gives Random famous phrase with author, picture and description'
  s.authors     = ['Asta Bevainyte']
  s.email       = 'asta.bevainyte@gmail.com'
  s.files       = ['lib/random_famous_phrase.rb']
  s.homepage    = 'http://rubygems.org/gems/random_famous_phrase'
  s.license     = 'MIT'
end
```
How to build gem?
____________________
% gem build random_famous_phrase.gemspec
```
Successfully built RubyGem
Name: random_famous_phrase
Version: 0.0.0
````
How to install gem  and test it works localy?
_________________________________
% gem install ./random_famous_phrase-0.0.0.gem
```
Successfully installed random_famous_phrase-0.0.0
Parsing documentation for random_famous_phrase-0.0.0
Installing ri documentation for random_famous_phrase-0.0.0
Done installing documentation for random_famous_phrase after 0 seconds
1 gem installed
```
% irb
```
2.1.3 :003 > require 'random_famous_phrase'
 => true 
2.1.3 :003 > RandomFamousPhrase.show
It should work - By Asta
 => nil 

```

