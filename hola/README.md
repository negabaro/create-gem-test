http://ruby-korea.github.io/rubygems-guides/make-your-own-gem/


.gemspec의 Name을 고유의 이름으로 바꿔줘야함


gem build hola.gemspec

hola-0.0.1.gem이 만들어짐

gem install ./hola-0.0.1.gem


irb
irb(main):001:0> require 'hola'
=> true


 Hola.hi('spanish')
=> "hola mundo"

Hola.hi('korean')
=> "anyoung ha se yo"

Hola.hi('sadsad')
=> "hello world"



curl -u qrush https://rubygems.org/api/v1/api_key.yaml > ~/.gem/credentials; chmod 0600 ~/.gem/credentials


gem push hola_negabaro-0.0.1.gem